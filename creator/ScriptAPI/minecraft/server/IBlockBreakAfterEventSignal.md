---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.IBlockBreakAfterEventSignal Class
description: Contents of the @minecraft/server.IBlockBreakAfterEventSignal class.
---
# IBlockBreakAfterEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Classes that extend IBlockBreakAfterEventSignal
- [*BlockBreakAfterEventSignal*](BlockBreakAfterEventSignal.md)

Provides an adaptable interface for callers to subscribe to an event that fires when blocks are broken.

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: BlockBreakAfterEvent) => void): (arg: BlockBreakAfterEvent) => void
`

#### **Parameters**
- **callback**: (arg: [*BlockBreakAfterEvent*](BlockBreakAfterEvent.md)) => *void*

#### **Returns** (arg: [*BlockBreakAfterEvent*](BlockBreakAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: BlockBreakAfterEvent) => void): void
`

#### **Parameters**
- **callback**: (arg: [*BlockBreakAfterEvent*](BlockBreakAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
