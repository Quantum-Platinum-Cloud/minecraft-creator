---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.IItemUseOnBeforeEventSignal Class
description: Contents of the @minecraft/server.IItemUseOnBeforeEventSignal class.
---
# IItemUseOnBeforeEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Classes that extend IItemUseOnBeforeEventSignal
- [*ItemUseOnBeforeEventSignal*](ItemUseOnBeforeEventSignal.md)

Provides an adaptable interface for callers to subscribe to an event that fires before an item is being used on a block.

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: ItemUseOnBeforeEvent) => void): (arg: ItemUseOnBeforeEvent) => void
`

#### **Parameters**
- **callback**: (arg: [*ItemUseOnBeforeEvent*](ItemUseOnBeforeEvent.md)) => *void*

#### **Returns** (arg: [*ItemUseOnBeforeEvent*](ItemUseOnBeforeEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: ItemUseOnBeforeEvent) => void): void
`

#### **Parameters**
- **callback**: (arg: [*ItemUseOnBeforeEvent*](ItemUseOnBeforeEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
