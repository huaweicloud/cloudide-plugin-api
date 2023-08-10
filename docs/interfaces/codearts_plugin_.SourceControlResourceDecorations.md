[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / SourceControlResourceDecorations

# Interface: SourceControlResourceDecorations

["@codearts/plugin"](../modules/_codearts_plugin_.md).SourceControlResourceDecorations

The decorations for a [source control resource state](codearts_plugin_.SourceControlResourceState.md).
Can be independently specified for light and dark themes.

## Hierarchy

- [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

  ↳ **`SourceControlResourceDecorations`**

## Table of contents

### Properties

- [dark](codearts_plugin_.SourceControlResourceDecorations.md#dark)
- [faded](codearts_plugin_.SourceControlResourceDecorations.md#faded)
- [iconPath](codearts_plugin_.SourceControlResourceDecorations.md#iconpath)
- [light](codearts_plugin_.SourceControlResourceDecorations.md#light)
- [strikeThrough](codearts_plugin_.SourceControlResourceDecorations.md#strikethrough)
- [tooltip](codearts_plugin_.SourceControlResourceDecorations.md#tooltip)

## Properties

### dark

• `Optional` `Readonly` **dark**: [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

The dark theme decorations.

#### Defined in

[index.d.ts:14828](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14828)

___

### faded

• `Optional` `Readonly` **faded**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be faded in the UI.

#### Defined in

[index.d.ts:14812](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14812)

___

### iconPath

• `Optional` `Readonly` **iconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md)

The icon path for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Inherited from

[SourceControlResourceThemableDecorations](codearts_plugin_.SourceControlResourceThemableDecorations.md).[iconPath](codearts_plugin_.SourceControlResourceThemableDecorations.md#iconpath)

#### Defined in

[index.d.ts:14793](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14793)

___

### light

• `Optional` `Readonly` **light**: [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

The light theme decorations.

#### Defined in

[index.d.ts:14823](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14823)

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be striked-through in the UI.

#### Defined in

[index.d.ts:14806](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14806)

___

### tooltip

• `Optional` `Readonly` **tooltip**: `string`

The title for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14818](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L14818)
