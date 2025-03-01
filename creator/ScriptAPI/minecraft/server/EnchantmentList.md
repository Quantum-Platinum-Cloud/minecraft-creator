---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.EnchantmentList Class
description: Contents of the @minecraft/server.EnchantmentList class.
---
# EnchantmentList Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Implements
- Iterator&lt;[*Enchantment*](Enchantment.md)&gt;

This class represents a collection of enchantments that can be applied to an item.

## Properties

### **slot**
`read-only slot: number;`

The item slot/type that this collection is applied to.

Type: *number*

## Methods
- [constructor](#constructor)
- [[Symbol.iterator]](#[symbol.iterator])
- [addEnchantment](#addenchantment)
- [canAddEnchantment](#canaddenchantment)
- [getEnchantment](#getenchantment)
- [hasEnchantment](#hasenchantment)
- [next](#next)
- [removeEnchantment](#removeenchantment)

### **constructor**
`
new EnchantmentList(enchantmentSlot: number)
`

Creates a new EnchantmentList.

#### **Parameters**
- **enchantmentSlot**: *number*

#### **Returns** [*EnchantmentList*](EnchantmentList.md)

### **[Symbol.iterator]**
`
[Symbol.iterator](): Iterator<Enchantment>
`

#### **Returns** Iterator&lt;[*Enchantment*](Enchantment.md)&gt;

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **addEnchantment**
`
addEnchantment(enchantment: Enchantment): boolean
`

Attempts to add the enchantment to this collection. Returns true if successful.

#### **Parameters**
- **enchantment**: [*Enchantment*](Enchantment.md)

#### **Returns** *boolean*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **canAddEnchantment**
`
canAddEnchantment(enchantment: Enchantment): boolean
`

Returns whether or not the provided EnchantmentInstance can be added to this collection.

#### **Parameters**
- **enchantment**: [*Enchantment*](Enchantment.md)

#### **Returns** *boolean*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **getEnchantment**
`
getEnchantment(enchantmentType: EnchantmentType | string): Enchantment | undefined
`

Returns an enchantment associated with a type.

#### **Parameters**
- **enchantmentType**: [*EnchantmentType*](EnchantmentType.md) | *string*

#### **Returns** [*Enchantment*](Enchantment.md) | *undefined*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.

### **hasEnchantment**
`
hasEnchantment(enchantmentType: EnchantmentType | string): number
`

If this collection has an EnchantmentInstance with type, returns the level of the enchantment. Returns 0 if not present.

#### **Parameters**
- **enchantmentType**: [*EnchantmentType*](EnchantmentType.md) | *string*

#### **Returns** *number*

> [!WARNING]
> This function can throw errors.

### **next**
`
next(): IteratorResult<Enchantment>
`

#### **Returns** IteratorResult&lt;[*Enchantment*](Enchantment.md)&gt;

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **removeEnchantment**
`
removeEnchantment(enchantmentType: EnchantmentType | string): void
`

Removes an EnchantmentInstance with type from this collection if present.

#### **Parameters**
- **enchantmentType**: [*EnchantmentType*](EnchantmentType.md) | *string*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
