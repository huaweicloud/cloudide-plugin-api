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

[index.d.ts:14799](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14799)

___

### faded

• `Optional` `Readonly` **faded**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be faded in the UI.

#### Defined in

[index.d.ts:14783](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14783)

___

### iconPath

• `Optional` `Readonly` **iconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md)

The icon path for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Inherited from

[SourceControlResourceThemableDecorations](codearts_plugin_.SourceControlResourceThemableDecorations.md).[iconPath](codearts_plugin_.SourceControlResourceThemableDecorations.md#iconpath)

#### Defined in

[index.d.ts:14764](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14764)

___

### light

• `Optional` `Readonly` **light**: [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

The light theme decorations.

#### Defined in

[index.d.ts:14794](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14794)

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be striked-through in the UI.

#### Defined in

[index.d.ts:14777](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14777)

___

### tooltip

• `Optional` `Readonly` **tooltip**: `string`

The title for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14789](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L14789)
