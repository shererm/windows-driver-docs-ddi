---
UID: NN:dbgmodel.IIterableConcept
title: IIterableConcept (dbgmodel.h)
description: The object is a container and can be iterated.
ms.date: 07/16/2018
keywords: ["IIterableConcept interface"]
req.header: dbgmodel.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
targetos: Windows
tech.root: debugger
ms.custom: RS5
f1_keywords:
 - IIterableConcept
 - dbgmodel/IIterableConcept
topic_type:
 - apiref
api_type:
 - COM
api_location:
 - dbgmodel.h
api_name:
 - IIterableConcept
---

# IIterableConcept interface


## -description

The object is a container and can be iterated.

## -inheritance

IIterableConcept inherits from IUnknown.

## -remarks

**Iterable Concept**

An object which is a container of other objects and wishes to express the ability to iterate over those contained objects can support the iterable concept by an implementation of the IIterableConcept and [IModelIterator](nn-dbgmodel-imodeliterator.md) interfaces. There is a very important relationship between support of the iterable concept and support of the indexable concept. An object which supports random access to the contained objects can support the indexable concept in addition to the iterable concept. In this case, the iterated elements must also produce a default index which, when passed to the indexable concept refer to the same object. A failure to satisfy this invariant will result in undefined behavior in the debug host.

## -see-also

[Debugger Data Model C++ Overview](/windows-hardware/drivers/debugger/data-model-cpp-overview)
