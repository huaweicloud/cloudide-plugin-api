**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ThemableDecorationRenderOptions

# Interface: ThemableDecorationRenderOptions

Represents theme specific rendering styles for a [text editor decoration](#TextEditorDecorationType).

## Hierarchy

* **ThemableDecorationRenderOptions**

  ↳ [DecorationRenderOptions](_index_d_._plugin_.decorationrenderoptions.md)

## Index

### Properties

* [after](_index_d_._plugin_.themabledecorationrenderoptions.md#after)
* [backgroundColor](_index_d_._plugin_.themabledecorationrenderoptions.md#backgroundcolor)
* [before](_index_d_._plugin_.themabledecorationrenderoptions.md#before)
* [border](_index_d_._plugin_.themabledecorationrenderoptions.md#border)
* [borderColor](_index_d_._plugin_.themabledecorationrenderoptions.md#bordercolor)
* [borderRadius](_index_d_._plugin_.themabledecorationrenderoptions.md#borderradius)
* [borderSpacing](_index_d_._plugin_.themabledecorationrenderoptions.md#borderspacing)
* [borderStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#borderstyle)
* [borderWidth](_index_d_._plugin_.themabledecorationrenderoptions.md#borderwidth)
* [color](_index_d_._plugin_.themabledecorationrenderoptions.md#color)
* [cursor](_index_d_._plugin_.themabledecorationrenderoptions.md#cursor)
* [fontStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#fontstyle)
* [fontWeight](_index_d_._plugin_.themabledecorationrenderoptions.md#fontweight)
* [gutterIconPath](_index_d_._plugin_.themabledecorationrenderoptions.md#guttericonpath)
* [gutterIconSize](_index_d_._plugin_.themabledecorationrenderoptions.md#guttericonsize)
* [letterSpacing](_index_d_._plugin_.themabledecorationrenderoptions.md#letterspacing)
* [opacity](_index_d_._plugin_.themabledecorationrenderoptions.md#opacity)
* [outline](_index_d_._plugin_.themabledecorationrenderoptions.md#outline)
* [outlineColor](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinecolor)
* [outlineStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinestyle)
* [outlineWidth](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinewidth)
* [overviewRulerColor](_index_d_._plugin_.themabledecorationrenderoptions.md#overviewrulercolor)
* [textDecoration](_index_d_._plugin_.themabledecorationrenderoptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [ThemableDecorationAttachmentRenderOptions](_index_d_._plugin_.themabledecorationattachmentrenderoptions.md)

*Defined in [index.d.ts:1078](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1078)*

Defines the rendering options of the attachment that is inserted after the decorated text.

___

### backgroundColor

• `Optional` **backgroundColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:958](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L958)*

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](#ThemeColor).

___

### before

• `Optional` **before**: [ThemableDecorationAttachmentRenderOptions](_index_d_._plugin_.themabledecorationattachmentrenderoptions.md)

*Defined in [index.d.ts:1073](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1073)*

Defines the rendering options of the attachment that is inserted before the decorated text.

___

### border

• `Optional` **border**: string

*Defined in [index.d.ts:986](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L986)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### borderColor

• `Optional` **borderColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:992](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L992)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderRadius

• `Optional` **borderRadius**: string

*Defined in [index.d.ts:998](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L998)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderSpacing

• `Optional` **borderSpacing**: string

*Defined in [index.d.ts:1004](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1004)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderStyle

• `Optional` **borderStyle**: string

*Defined in [index.d.ts:1010](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1010)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderWidth

• `Optional` **borderWidth**: string

*Defined in [index.d.ts:1016](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1016)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### color

• `Optional` **color**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:1041](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1041)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### cursor

• `Optional` **cursor**: string

*Defined in [index.d.ts:1036](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1036)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### fontStyle

• `Optional` **fontStyle**: string

*Defined in [index.d.ts:1021](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1021)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### fontWeight

• `Optional` **fontWeight**: string

*Defined in [index.d.ts:1026](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1026)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### gutterIconPath

• `Optional` **gutterIconPath**: string \| [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1056](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1056)*

An **absolute path** or an URI to an image to be rendered in the gutter.

___

### gutterIconSize

• `Optional` **gutterIconSize**: string

*Defined in [index.d.ts:1063](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1063)*

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

___

### letterSpacing

• `Optional` **letterSpacing**: string

*Defined in [index.d.ts:1051](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1051)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### opacity

• `Optional` **opacity**: string

*Defined in [index.d.ts:1046](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1046)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### outline

• `Optional` **outline**: string

*Defined in [index.d.ts:963](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L963)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### outlineColor

• `Optional` **outlineColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:969](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L969)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### outlineStyle

• `Optional` **outlineStyle**: string

*Defined in [index.d.ts:975](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L975)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### outlineWidth

• `Optional` **outlineWidth**: string

*Defined in [index.d.ts:981](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L981)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Defined in [index.d.ts:1068](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1068)*

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

___

### textDecoration

• `Optional` **textDecoration**: string

*Defined in [index.d.ts:1031](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L1031)*

CSS styling property that will be applied to text enclosed by a decoration.
