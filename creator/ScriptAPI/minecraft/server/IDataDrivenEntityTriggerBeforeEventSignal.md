---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.IDataDrivenEntityTriggerBeforeEventSignal Class
description: Contents of the @minecraft/server.IDataDrivenEntityTriggerBeforeEventSignal class.
---
# IDataDrivenEntityTriggerBeforeEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Classes that extend IDataDrivenEntityTriggerBeforeEventSignal
- [*DataDrivenEntityTriggerBeforeEventSignal*](DataDrivenEntityTriggerBeforeEventSignal.md)

Provides an adaptable interface for callers to subscribe to an event that fires before an entities' definition is scheduled to change via a triggered event.

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: DataDrivenEntityTriggerBeforeEvent) => void, options?: EntityDataDrivenTriggerEventOptions): (arg: DataDrivenEntityTriggerBeforeEvent) => void
`

#### **Parameters**
- **callback**: (arg: [*DataDrivenEntityTriggerBeforeEvent*](DataDrivenEntityTriggerBeforeEvent.md)) => *void*
- **options**?: [*EntityDataDrivenTriggerEventOptions*](EntityDataDrivenTriggerEventOptions.md) = `null`

#### **Returns** (arg: [*DataDrivenEntityTriggerBeforeEvent*](DataDrivenEntityTriggerBeforeEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: DataDrivenEntityTriggerBeforeEvent) => void): void
`

#### **Parameters**
- **callback**: (arg: [*DataDrivenEntityTriggerBeforeEvent*](DataDrivenEntityTriggerBeforeEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
