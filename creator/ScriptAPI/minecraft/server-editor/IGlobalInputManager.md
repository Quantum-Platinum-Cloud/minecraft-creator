---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server-editor.IGlobalInputManager Interface
description: Contents of the @minecraft/server-editor.IGlobalInputManager class.
---
# IGlobalInputManager Interface

@beta

## Methods
- [registerKeyBinding](#registerkeybinding)

### **registerKeyBinding**
`
registerKeyBinding(inputContextId: EditorInputContext, action: SupportedKeyboardActionTypes, button: KeyboardKey, modifier: InputModifier): void
`

Register a key press binding for an action which will be handled by the specified input context.

#### **Parameters**
- **inputContextId**: *EditorInputContext*
  
  Id of the UI context to handle this binding.
- **action**: *SupportedKeyboardActionTypes*
  
  Action to register the binding for.
- **button**: *KeyboardKey*
  
  Keyboard key to invoke action.
- **modifier**: *InputModifier*
  
  Modifiers to create an input binding chord (Default: None).

#### **Returns** *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.
