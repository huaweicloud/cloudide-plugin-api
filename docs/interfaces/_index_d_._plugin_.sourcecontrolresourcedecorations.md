**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SourceControlResourceDecorations

# Interface: SourceControlResourceDecorations

The decorations for a [source control resource state](#SourceControlResourceState).
Can be independently specified for light and dark themes.

## Hierarchy

* [SourceControlResourceThemableDecorations](_index_d_._plugin_.sourcecontrolresourcethemabledecorations.md)

  ↳ **SourceControlResourceDecorations**

## Index

### Properties

* [dark](_index_d_._plugin_.sourcecontrolresourcedecorations.md#dark)
* [faded](_index_d_._plugin_.sourcecontrolresourcedecorations.md#faded)
* [iconPath](_index_d_._plugin_.sourcecontrolresourcedecorations.md#iconpath)
* [light](_index_d_._plugin_.sourcecontrolresourcedecorations.md#light)
* [strikeThrough](_index_d_._plugin_.sourcecontrolresourcedecorations.md#strikethrough)
* [tooltip](_index_d_._plugin_.sourcecontrolresourcedecorations.md#tooltip)

## Properties

### dark

• `Optional` `Readonly` **dark**: [SourceControlResourceThemableDecorations](_index_d_._plugin_.sourcecontrolresourcethemabledecorations.md)

*Defined in [index.d.ts:11286](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11286)*

The dark theme decorations.

___

### faded

• `Optional` `Readonly` **faded**: boolean

*Defined in [index.d.ts:11270](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11270)*

Whether the [source control resource state](#SourceControlResourceState) should
be faded in the UI.

___

### iconPath

• `Optional` `Readonly` **iconPath**: string \| [Uri](../classes/_index_d_._plugin_.uri.md)

*Inherited from [SourceControlResourceThemableDecorations](_index_d_._plugin_.sourcecontrolresourcethemabledecorations.md).[iconPath](_index_d_._plugin_.sourcecontrolresourcethemabledecorations.md#iconpath)*

*Defined in [index.d.ts:11251](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11251)*

The icon path for a specific
[source control resource state](#SourceControlResourceState).

___

### light

• `Optional` `Readonly` **light**: [SourceControlResourceThemableDecorations](_index_d_._plugin_.sourcecontrolresourcethemabledecorations.md)

*Defined in [index.d.ts:11281](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11281)*

The light theme decorations.

___

### strikeThrough

• `Optional` `Readonly` **strikeThrough**: boolean

*Defined in [index.d.ts:11264](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11264)*

Whether the [source control resource state](#SourceControlResourceState) should
be striked-through in the UI.

___

### tooltip

• `Optional` `Readonly` **tooltip**: string

*Defined in [index.d.ts:11276](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11276)*

The title for a specific
[source control resource state](#SourceControlResourceState).
