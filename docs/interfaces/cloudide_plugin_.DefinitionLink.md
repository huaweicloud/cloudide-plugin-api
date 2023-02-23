[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DefinitionLink

# Interface: DefinitionLink

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DefinitionLink

Information about where a symbol is defined.

Provides additional metadata over normal [location](#Location) definitions, including the range of
the defining symbol

## Table of contents

### Properties

- [originSelectionRange](cloudide_plugin_.DefinitionLink.md#originselectionrange)
- [targetRange](cloudide_plugin_.DefinitionLink.md#targetrange)
- [targetSelectionRange](cloudide_plugin_.DefinitionLink.md#targetselectionrange)
- [targetUri](cloudide_plugin_.DefinitionLink.md#targeturi)

## Properties

### originSelectionRange

• `Optional` **originSelectionRange**: [`Range`](../classes/cloudide_plugin_.Range.md)

Span of the symbol being defined in the source file.

Used as the underlined span for mouse definition hover. Defaults to the word range at
the definition position.

#### Defined in

[index.d.ts:689](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L689)

___

### targetRange

• **targetRange**: [`Range`](../classes/cloudide_plugin_.Range.md)

The full range of the definition.

For a class definition for example, this would be the entire body of the class definition.

#### Defined in

[index.d.ts:701](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L701)

___

### targetSelectionRange

• `Optional` **targetSelectionRange**: [`Range`](../classes/cloudide_plugin_.Range.md)

The span of the symbol definition.

For a class definition, this would be the class name itself in the class definition.

#### Defined in

[index.d.ts:708](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L708)

___

### targetUri

• **targetUri**: [`Uri`](../classes/cloudide_plugin_.Uri.md)

The resource identifier of the definition.

#### Defined in

[index.d.ts:694](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L694)
