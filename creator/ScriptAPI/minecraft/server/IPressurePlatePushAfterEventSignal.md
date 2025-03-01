---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.IPressurePlatePushAfterEventSignal Class
description: Contents of the @minecraft/server.IPressurePlatePushAfterEventSignal class.
---
# IPressurePlatePushAfterEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Classes that extend IPressurePlatePushAfterEventSignal
- [*PressurePlatePushAfterEventSignal*](PressurePlatePushAfterEventSignal.md)

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: PressurePlatePushAfterEvent) => void): (arg: PressurePlatePushAfterEvent) => void
`

#### **Parameters**
- **callback**: (arg: [*PressurePlatePushAfterEvent*](PressurePlatePushAfterEvent.md)) => *void*

#### **Returns** (arg: [*PressurePlatePushAfterEvent*](PressurePlatePushAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: PressurePlatePushAfterEvent) => void): void
`

#### **Parameters**
- **callback**: (arg: [*PressurePlatePushAfterEvent*](PressurePlatePushAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
