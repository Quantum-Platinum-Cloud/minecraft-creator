---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.ScoreboardIdentity Class
description: Contents of the @minecraft/server.ScoreboardIdentity class.
---
# ScoreboardIdentity Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

Contains an identity of the scoreboard item.

## Properties

### **displayName**
`read-only displayName: string;`

Returns the player-visible name of this identity.

Type: *string*

### **id**
`read-only id: number;`

Identifier of the scoreboard identity.

Type: *number*

### **type**
`read-only type: ScoreboardIdentityType;`

Type of the scoreboard identity.

Type: [*ScoreboardIdentityType*](ScoreboardIdentityType.md)

## Methods
- [getEntity](#getentity)
- [isValid](#isvalid)

### **getEntity**
`
getEntity(): Entity
`

If the scoreboard identity is an entity or player, returns the entity that this scoreboard item corresponds to.

#### **Returns** [*Entity*](Entity.md)

> [!WARNING]
> This function can throw errors.

### **isValid**
`
isValid(): boolean
`

#### **Returns** *boolean*
