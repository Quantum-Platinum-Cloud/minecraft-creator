---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.PropertyRegistry Class
description: Contents of the @minecraft/server.PropertyRegistry class.
---
# PropertyRegistry Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

Provides methods that should be used within the World Initialize event to register dynamic properties that can be used and stored within Minecraft.

## Methods
- [registerEntityTypeDynamicProperties](#registerentitytypedynamicproperties)
- [registerWorldDynamicProperties](#registerworlddynamicproperties)

### **registerEntityTypeDynamicProperties**
`
registerEntityTypeDynamicProperties(propertiesDefinition: DynamicPropertiesDefinition, entityType: EntityType): void
`

Registers a dynamic property for a particular entity type (e.g., a minecraft:skeleton.).

#### **Parameters**
- **propertiesDefinition**: [*DynamicPropertiesDefinition*](DynamicPropertiesDefinition.md)
- **entityType**: [*EntityType*](EntityType.md)

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.

### **registerWorldDynamicProperties**
`
registerWorldDynamicProperties(propertiesDefinition: DynamicPropertiesDefinition): void
`

Registers a globally available dynamic property for a world.

#### **Parameters**
- **propertiesDefinition**: [*DynamicPropertiesDefinition*](DynamicPropertiesDefinition.md)

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
