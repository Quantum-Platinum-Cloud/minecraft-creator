---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.IEntityRemovedAfterEventSignal Class
description: Contents of the @minecraft/server.IEntityRemovedAfterEventSignal class.
---
# IEntityRemovedAfterEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Classes that extend IEntityRemovedAfterEventSignal
- [*EntityRemovedAfterEventSignal*](EntityRemovedAfterEventSignal.md)

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: EntityRemovedAfterEvent) => void, options?: EntityEventOptions): (arg: EntityRemovedAfterEvent) => void
`

#### **Parameters**
- **callback**: (arg: [*EntityRemovedAfterEvent*](EntityRemovedAfterEvent.md)) => *void*
- **options**?: [*EntityEventOptions*](EntityEventOptions.md) = `null`

#### **Returns** (arg: [*EntityRemovedAfterEvent*](EntityRemovedAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: EntityRemovedAfterEvent) => void): void
`

#### **Parameters**
- **callback**: (arg: [*EntityRemovedAfterEvent*](EntityRemovedAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
