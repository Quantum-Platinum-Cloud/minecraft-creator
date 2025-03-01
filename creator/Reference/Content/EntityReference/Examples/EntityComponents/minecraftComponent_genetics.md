---
author: mammerla
ms.author: v-jimseaman
title: Entity Documentation - minecraft:genetics
ms.prod: gaming
---

# Entity Documentation - minecraft:genetics

`minecraft:genetics` defines the way a mob's genes and alleles are passed on to its offspring, and how those traits manifest in the child. Compatible parent genes are crossed together, the alleles are handed down from the parents to the child, and any matching genetic variants initiate JSON events to modify the child and express the traits.

## Parameters

|Name |Default Value  |Type  |Description  |
|:----------|:----------|:----------|:----------|
| genes| *not set*| List| The list of genes that this entity has and will cross with a partner during breeding.|
| mutation_rate| 0.03125| Decimal| Chance that an allele will be replaced with a random one instead of the parent's allele during birth. |
| use_simplified_breeding| --| Boolean| When set to 'true', this optional flag prohibits the inheritance of hidden parent alleles as main alleles in children and the inheritance of main alleles as hidden alleles in children. This allows for easier implementation of basic breeding logic. |

### genes

`genes` is a list defined by three parameters. Each item has the following properties:

| Name| Default Value| Type| Description |
|:----------|:----------|:----------|:----------|
| allele_range| *not set*| Integer| The range of positive integer allele values for this gene. Spawned mobs will have a random number in this range assigned to them.|
| genetic_variants| *not set*| List| The list of genetic variants for this gene. These check for particular allele combinations and initiate events when all of them are satisfied.|
| name| *not set*| String| The name of the gene. |

#### allele_range

`allele_range` is an integer defined by two parameters. Each item has the following properties:

| Name| Default Value| Type| Description |
|:-----------|:-----------|:-----------|:-----------|
| range_max| 0| Integer| Upper bound of the allele values for this gene. |
| range_min| 0| Integer| Lower bound of the allele values for this gene. |

#### genetic_variants

`genetic_variants` is a decimal defined by five parameters. Each item has the following properties:

| Name| Default Value| Type| Description |
|:-----------|:-----------|:-----------|:-----------|
| birth_event| *not set*| JSON Object| Event to run when this mob is created and matches the allele conditions. |
| both_allele| -1| Integer| If this value is non-negative, compare both the mob's main and hidden alleles with this value for a match with both. Can also be a range of integers. |
| either_allele| -1| Integer| If this value is non-negative, compare both the mob's main and hidden alleles with this value for a match with either. Can also be a range of integers. |
| hidden_allele| -1| Integer| If this value is non-negative, compare the mob's hidden allele with this value for a match. Can also be a range of integers. |
| main_allele| -1| Integer| If this value is non-negative, compare the mob's main allele with this value for a match. Can also be a range of integers. |
| mutation_rate| -1| Decimal| If this value is non-negative, overrides the chance for this gene that an allele will be replaced with a random one instead of the parent's allele during birth. Non-negative values greater than `1` will be the same as the value `1`. |

## Example

```json
"minecraft:genetics":{
    "genes": [
        {
            "allele_range": {
                "range_max": 0,
                "range_min": 0,
            },
            "genetic_variants": [
                {
                    "birth_event": {
                      "event": "minecraft:born_screamer",
                      "target": "self"
                    },                    
                    "main_allele": {
                      "range_min": 1,
                      "range_max": 2
                    }
                }
            ],
            "name": "gene",
        }
    ],
    "mutation_rate": 0.03125
}
```

## Vanilla entities examples

### panda

```json
"mutation_rate": 0.03125,
        "genes": [
          {
            "name": "panda_variant",
            "allele_range": {
              "range_min": 0,
              "range_max": 15
            },
            "genetic_variants": [
              {
                "main_allele": 0,
                "birth_event": {
                  "event": "minecraft:panda_lazy",
                  "target": "self"
                }
              },
              {
                "main_allele": 1,
                "birth_event": {
                  "event": "minecraft:panda_worried",
                  "target": "self"
                }
              },
              {
                "main_allele": 2,
                "birth_event": {
                  "event": "minecraft:panda_playful",
                  "target": "self"
                }
              },
              {
                "main_allele": 3,
                "birth_event": {
                  "event": "minecraft:panda_aggressive",
                  "target": "self"
                }
              },
              {
                "both_allele": {
                  "range_min": 4,
                  "range_max": 7
                },
                "birth_event": {
                  "event": "minecraft:panda_weak",
                  "target": "self"
                }
              },
              {
                "both_allele": {
                  "range_min": 8,
                  "range_max": 9
                },
                "birth_event": {
                  "event": "minecraft:panda_brown",
                  "target": "self"
                }
              }
            ]
          }
        ]
```

## Vanilla entities using `minecraft:genetics`

- [goat](../../../../Source/VanillaBehaviorPack_Snippets/entities/goat.md)
- [panda](../../../../Source/VanillaBehaviorPack_Snippets/entities/panda.md)