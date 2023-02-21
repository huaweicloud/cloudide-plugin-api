[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / SourceControlResourceDecorations

# Interface: SourceControlResourceDecorations

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).SourceControlResourceDecorations

The decorations for a [source control resource state](#SourceControlResourceState).
Can be independently specified for light and dark themes.

## Hierarchy

- [`SourceControlResourceThemableDecorations`](cloudide_plugin_.SourceControlResourceThemableDecorations.md)

  ↳ **`SourceControlResourceDecorations`**

## Table of contents

### Properties

- [dark](cloudide_plugin_.SourceControlResourceDecorations.md#dark)
- [faded](cloudide_plugin_.SourceControlResourceDecorations.md#faded)
- [iconPath](cloudide_plugin_.SourceControlResourceDecorations.md#iconpath)
- [light](cloudide_plugin_.SourceControlResourceDecorations.md#light)
- [strikeThrough](cloudide_plugin_.SourceControlResourceDecorations.md#strikethrough)
- [tooltip](cloudide_plugin_.SourceControlResourceDecorations.md#tooltip)

## Properties

### dark

• `Optional` `Readonly` **dark**: [`SourceControlResourceThemableDecorations`](cloudide_plugin_.SourceControlResourceThemableDecorations.md)

The dark theme decorations.

#### Defined in

[index.d.ts:9386](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9386)

___

### faded

• `Optional` `Readonly` **faded**: `boolean`

Whether the [source control resource state](#SourceControlResourceState) should
be faded in the UI.

#### Defined in

[index.d.ts:9370](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9370)

___

### iconPath

• `Optional` `Readonly` **iconPath**: `string` \| [`Uri`](../classes/cloudide_plugin_.Uri.md)

The icon path for a specific
[source control resource state](#SourceControlResourceState).

#### Inherited from

[SourceControlResourceThemableDecorations](cloudide_plugin_.SourceControlResourceThemableDecorations.md).[iconPath](cloudide_plugin_.SourceControlResourceThemableDecorations.md#iconpath)

#### Defined in

[index.d.ts:9351](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9351)

___

### light

• `Optional` `Readonly` **light**: [`SourceControlResourceThemableDecorations`](cloudide_plugin_.SourceControlResourceThemableDecorations.md)

The light theme decorations.

#### Defined in

[index.d.ts:9381](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9381)

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: `boolean`

Whether the [source control resource state](#SourceControlResourceState) should
be striked-through in the UI.

#### Defined in

[index.d.ts:9364](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9364)

___

### tooltip

• `Optional` `Readonly` **tooltip**: `string`

The title for a specific
[source control resource state](#SourceControlResourceState).

#### Defined in

[index.d.ts:9376](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9376)
