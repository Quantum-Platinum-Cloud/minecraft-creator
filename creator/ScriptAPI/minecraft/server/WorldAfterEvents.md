---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.WorldAfterEvents Class
description: Contents of the @minecraft/server.WorldAfterEvents class.
---
# WorldAfterEvents Class

Contains a set of events that are available across the scope of the World.

## Properties

### **blockBreak**
`read-only blockBreak: BlockBreakAfterEventSignal;`

This event fires for a block that is broken by a player.

Type: [*BlockBreakAfterEventSignal*](BlockBreakAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **blockExplode**
`read-only blockExplode: BlockExplodeAfterEventSignal;`

This event fires for each BlockLocation destroyed by an explosion. It is fired after the blocks have already been destroyed.

Type: [*BlockExplodeAfterEventSignal*](BlockExplodeAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **blockPlace**
`read-only blockPlace: BlockPlaceAfterEventSignal;`

This event fires for a block that is placed by a player.

Type: [*BlockPlaceAfterEventSignal*](BlockPlaceAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **buttonPush**
`read-only buttonPush: ButtonPushAfterEventSignal;`

This event fires when a button is pushed.

Type: [*ButtonPushAfterEventSignal*](ButtonPushAfterEventSignal.md)

### **chatSend**
`read-only chatSend: ChatSendAfterEventSignal;`

This event is triggered after a chat message has been broadcast or sent to players.

Type: [*ChatSendAfterEventSignal*](ChatSendAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **dataDrivenEntityTriggerEvent**
`read-only dataDrivenEntityTriggerEvent: DataDrivenEntityTriggerAfterEventSignal;`

This event is fired when an entity event has been triggered that will update the component definition state of an entity.

Type: [*DataDrivenEntityTriggerAfterEventSignal*](DataDrivenEntityTriggerAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **effectAdd**
`read-only effectAdd: EffectAddAfterEventSignal;`

This event fires when an effect, like poisoning, is added to an entity.

Type: [*EffectAddAfterEventSignal*](EffectAddAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityDie**
`read-only entityDie: EntityDieAfterEventSignal;`

This event fires when an entity dies.

Type: [*EntityDieAfterEventSignal*](EntityDieAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityHealthChanged**
`read-only entityHealthChanged: EntityHealthChangedAfterEventSignal;`

This event fires when entity health changes in any degree.

Type: [*EntityHealthChangedAfterEventSignal*](EntityHealthChangedAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityHitBlock**
`read-only entityHitBlock: EntityHitBlockAfterEventSignal;`

This event fires when an entity hits (that is, melee attacks) a block.

Type: [*EntityHitBlockAfterEventSignal*](EntityHitBlockAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityHitEntity**
`read-only entityHitEntity: EntityHitEntityAfterEventSignal;`

This event fires when an entity hits (that is, melee attacks) another entity.

Type: [*EntityHitEntityAfterEventSignal*](EntityHitEntityAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityHurt**
`read-only entityHurt: EntityHurtAfterEventSignal;`

This event fires when an entity is hurt (takes damage).

Type: [*EntityHurtAfterEventSignal*](EntityHurtAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entityRemoved**
`read-only entityRemoved: EntityRemovedAfterEventSignal;`

This event fires when an entity is removed from the game (e.g., is unloaded when it goes out of range; or a few seconds after the death of an entity.)

Type: [*EntityRemovedAfterEventSignal*](EntityRemovedAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **entitySpawn**
`read-only entitySpawn: EntitySpawnAfterEventSignal;`

This event fires when an entity is spawned.

Type: [*EntitySpawnAfterEventSignal*](EntitySpawnAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **explosion**
`read-only explosion: ExplosionAfterEventSignal;`

This event is fired after an explosion occurs.

Type: [*ExplosionAfterEventSignal*](ExplosionAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemCompleteUse**
`read-only itemCompleteUse: ItemCompleteUseAfterEventSignal;`

This event fires when a chargeable item completes charging.

Type: [*ItemCompleteUseAfterEventSignal*](ItemCompleteUseAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemDefinitionEvent**
`read-only itemDefinitionEvent: ItemDefinitionAfterEventSignal;`

For custom items, this event is triggered when the fundamental set of defined components for the item change.  Note that this event is only fired for custom data-driven items.

Type: [*ItemDefinitionAfterEventSignal*](ItemDefinitionAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemReleaseUse**
`read-only itemReleaseUse: ItemReleaseUseAfterEventSignal;`

This event fires when a chargeable item is released from charging.

Type: [*ItemReleaseUseAfterEventSignal*](ItemReleaseUseAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemStartUse**
`read-only itemStartUse: ItemStartUseAfterEventSignal;`

This event fires when a chargeable item starts charging.

Type: [*ItemStartUseAfterEventSignal*](ItemStartUseAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemStartUseOn**
`read-only itemStartUseOn: ItemStartUseOnAfterEventSignal;`

This event fires when a player successfully uses an item or places a block by pressing the Use Item / Place Block button. If multiple blocks are placed, this event will only occur once at the beginning of the block placement. Note: This event cannot be used with Hoe or Axe items.

Type: [*ItemStartUseOnAfterEventSignal*](ItemStartUseOnAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemStopUse**
`read-only itemStopUse: ItemStopUseAfterEventSignal;`

This event fires when a chargeable item stops charging.

Type: [*ItemStopUseAfterEventSignal*](ItemStopUseAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemStopUseOn**
`read-only itemStopUseOn: ItemStopUseOnAfterEventSignal;`

This event fires when a player releases the Use Item / Place Block button after successfully using an item. Note: This event cannot be used with Hoe or Axe items.

Type: [*ItemStopUseOnAfterEventSignal*](ItemStopUseOnAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemUse**
`read-only itemUse: ItemUseAfterEventSignal;`

This event fires when an item is successfully used by a player.

Type: [*ItemUseAfterEventSignal*](ItemUseAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **itemUseOn**
`read-only itemUseOn: ItemUseOnAfterEventSignal;`

This event fires when an item is used on a block by a player.

Type: [*ItemUseOnAfterEventSignal*](ItemUseOnAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **leverAction**
`read-only leverAction: LeverActionAfterEventSignal;`

A lever has been pulled.

Type: [*LeverActionAfterEventSignal*](LeverActionAfterEventSignal.md)

### **messageReceive**
`read-only messageReceive: ServerMessageAfterEventSignal;`

This event is an internal implementation detail, and is otherwise not currently functional.

Type: [*ServerMessageAfterEventSignal*](ServerMessageAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **pistonActivate**
`read-only pistonActivate: PistonActivateAfterEventSignal;`

This event fires when a piston expands or retracts.

Type: [*PistonActivateAfterEventSignal*](PistonActivateAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **playerJoin**
`read-only playerJoin: PlayerJoinAfterEventSignal;`

This event fires when a player joins a world.  See also playerSpawn for another related event you can trap for when a player is spawned the first time within a world.

Type: [*PlayerJoinAfterEventSignal*](PlayerJoinAfterEventSignal.md)

### **playerLeave**
`read-only playerLeave: PlayerLeaveAfterEventSignal;`

This event fires when a player leaves a world.

Type: [*PlayerLeaveAfterEventSignal*](PlayerLeaveAfterEventSignal.md)

### **playerSpawn**
`read-only playerSpawn: PlayerSpawnAfterEventSignal;`

This event fires when a player spawns or respawns. Note that an additional flag within this event will tell you whether the player is spawning right after join vs. a respawn.

Type: [*PlayerSpawnAfterEventSignal*](PlayerSpawnAfterEventSignal.md)

### **pressurePlatePop**
`read-only pressurePlatePop: PressurePlatePopAfterEventSignal;`

A pressure plate has popped back up (i.e., there are no entities on the pressure plate.)

Type: [*PressurePlatePopAfterEventSignal*](PressurePlatePopAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **pressurePlatePush**
`read-only pressurePlatePush: PressurePlatePushAfterEventSignal;`

A pressure plate has pushed (at least one entity has moved onto a pressure plate.)

Type: [*PressurePlatePushAfterEventSignal*](PressurePlatePushAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **projectileHit**
`read-only projectileHit: ProjectileHitAfterEventSignal;`

This event fires when a projectile hits an entity or block.

Type: [*ProjectileHitAfterEventSignal*](ProjectileHitAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **targetBlockHit**
`read-only targetBlockHit: TargetBlockHitAfterEventSignal;`

A target block was hit.

Type: [*TargetBlockHitAfterEventSignal*](TargetBlockHitAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **tripWireTrip**
`read-only tripWireTrip: TripWireTripAfterEventSignal;`

A trip wire was tripped.

Type: [*TripWireTripAfterEventSignal*](TripWireTripAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **weatherChange**
`read-only weatherChange: WeatherChangeAfterEventSignal;`

This event will be triggered when the weather changes within Minecraft.

Type: [*WeatherChangeAfterEventSignal*](WeatherChangeAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.

### **worldInitialize**
`read-only worldInitialize: WorldInitializeAfterEventSignal;`

This event fires when the script environment is initialized on a World. In addition, you can register dynamic properties within the scope of a world Initialize event.

Type: [*WorldInitializeAfterEventSignal*](WorldInitializeAfterEventSignal.md)

> [!CAUTION]
> This property is still in pre-release.  Its signature may change or it may be removed in future releases.
