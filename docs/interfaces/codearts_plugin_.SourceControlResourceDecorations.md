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

[index.d.ts:14696](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14696)

___

### faded

• `Optional` `Readonly` **faded**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be faded in the UI.

#### Defined in

[index.d.ts:14680](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14680)

___

### iconPath

• `Optional` `Readonly` **iconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md)

The icon path for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Inherited from

[SourceControlResourceThemableDecorations](codearts_plugin_.SourceControlResourceThemableDecorations.md).[iconPath](codearts_plugin_.SourceControlResourceThemableDecorations.md#iconpath)

#### Defined in

[index.d.ts:14661](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14661)

___

### light

• `Optional` `Readonly` **light**: [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

The light theme decorations.

#### Defined in

[index.d.ts:14691](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14691)

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be striked-through in the UI.

#### Defined in

[index.d.ts:14674](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14674)

___

### tooltip

• `Optional` `Readonly` **tooltip**: `string`

The title for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14686](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L14686)
