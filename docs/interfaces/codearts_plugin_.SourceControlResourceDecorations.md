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

[index.d.ts:14644](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14644)

___

### faded

• `Optional` `Readonly` **faded**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be faded in the UI.

#### Defined in

[index.d.ts:14628](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14628)

___

### iconPath

• `Optional` `Readonly` **iconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md) \| [`ThemeIcon`](../classes/codearts_plugin_.ThemeIcon.md)

The icon path for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Inherited from

[SourceControlResourceThemableDecorations](codearts_plugin_.SourceControlResourceThemableDecorations.md).[iconPath](codearts_plugin_.SourceControlResourceThemableDecorations.md#iconpath)

#### Defined in

[index.d.ts:14609](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14609)

___

### light

• `Optional` `Readonly` **light**: [`SourceControlResourceThemableDecorations`](codearts_plugin_.SourceControlResourceThemableDecorations.md)

The light theme decorations.

#### Defined in

[index.d.ts:14639](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14639)

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: `boolean`

Whether the [source control resource state](codearts_plugin_.SourceControlResourceState.md) should
be striked-through in the UI.

#### Defined in

[index.d.ts:14622](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14622)

___

### tooltip

• `Optional` `Readonly` **tooltip**: `string`

The title for a specific
[source control resource state](codearts_plugin_.SourceControlResourceState.md).

#### Defined in

[index.d.ts:14634](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L14634)
