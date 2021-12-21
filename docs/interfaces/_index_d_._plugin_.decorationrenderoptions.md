**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DecorationRenderOptions

# Interface: DecorationRenderOptions

Represents rendering styles for a [text editor decoration](#TextEditorDecorationType).

## Hierarchy

* [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md)

  ↳ **DecorationRenderOptions**

## Index

### Properties

* [after](_index_d_._plugin_.decorationrenderoptions.md#after)
* [backgroundColor](_index_d_._plugin_.decorationrenderoptions.md#backgroundcolor)
* [before](_index_d_._plugin_.decorationrenderoptions.md#before)
* [border](_index_d_._plugin_.decorationrenderoptions.md#border)
* [borderColor](_index_d_._plugin_.decorationrenderoptions.md#bordercolor)
* [borderRadius](_index_d_._plugin_.decorationrenderoptions.md#borderradius)
* [borderSpacing](_index_d_._plugin_.decorationrenderoptions.md#borderspacing)
* [borderStyle](_index_d_._plugin_.decorationrenderoptions.md#borderstyle)
* [borderWidth](_index_d_._plugin_.decorationrenderoptions.md#borderwidth)
* [color](_index_d_._plugin_.decorationrenderoptions.md#color)
* [cursor](_index_d_._plugin_.decorationrenderoptions.md#cursor)
* [dark](_index_d_._plugin_.decorationrenderoptions.md#dark)
* [fontStyle](_index_d_._plugin_.decorationrenderoptions.md#fontstyle)
* [fontWeight](_index_d_._plugin_.decorationrenderoptions.md#fontweight)
* [gutterIconPath](_index_d_._plugin_.decorationrenderoptions.md#guttericonpath)
* [gutterIconSize](_index_d_._plugin_.decorationrenderoptions.md#guttericonsize)
* [isWholeLine](_index_d_._plugin_.decorationrenderoptions.md#iswholeline)
* [letterSpacing](_index_d_._plugin_.decorationrenderoptions.md#letterspacing)
* [light](_index_d_._plugin_.decorationrenderoptions.md#light)
* [opacity](_index_d_._plugin_.decorationrenderoptions.md#opacity)
* [outline](_index_d_._plugin_.decorationrenderoptions.md#outline)
* [outlineColor](_index_d_._plugin_.decorationrenderoptions.md#outlinecolor)
* [outlineStyle](_index_d_._plugin_.decorationrenderoptions.md#outlinestyle)
* [outlineWidth](_index_d_._plugin_.decorationrenderoptions.md#outlinewidth)
* [overviewRulerColor](_index_d_._plugin_.decorationrenderoptions.md#overviewrulercolor)
* [overviewRulerLane](_index_d_._plugin_.decorationrenderoptions.md#overviewrulerlane)
* [rangeBehavior](_index_d_._plugin_.decorationrenderoptions.md#rangebehavior)
* [textDecoration](_index_d_._plugin_.decorationrenderoptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [ThemableDecorationAttachmentRenderOptions](_index_d_._plugin_.themabledecorationattachmentrenderoptions.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[after](_index_d_._plugin_.themabledecorationrenderoptions.md#after)*

*Defined in [index.d.ts:1075](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1075)*

Defines the rendering options of the attachment that is inserted after the decorated text.

___

### backgroundColor

• `Optional` **backgroundColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[backgroundColor](_index_d_._plugin_.themabledecorationrenderoptions.md#backgroundcolor)*

*Defined in [index.d.ts:955](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L955)*

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](#ThemeColor).

___

### before

• `Optional` **before**: [ThemableDecorationAttachmentRenderOptions](_index_d_._plugin_.themabledecorationattachmentrenderoptions.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[before](_index_d_._plugin_.themabledecorationrenderoptions.md#before)*

*Defined in [index.d.ts:1070](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1070)*

Defines the rendering options of the attachment that is inserted before the decorated text.

___

### border

• `Optional` **border**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[border](_index_d_._plugin_.themabledecorationrenderoptions.md#border)*

*Defined in [index.d.ts:983](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L983)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### borderColor

• `Optional` **borderColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[borderColor](_index_d_._plugin_.themabledecorationrenderoptions.md#bordercolor)*

*Defined in [index.d.ts:989](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L989)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderRadius

• `Optional` **borderRadius**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[borderRadius](_index_d_._plugin_.themabledecorationrenderoptions.md#borderradius)*

*Defined in [index.d.ts:995](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L995)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderSpacing

• `Optional` **borderSpacing**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[borderSpacing](_index_d_._plugin_.themabledecorationrenderoptions.md#borderspacing)*

*Defined in [index.d.ts:1001](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1001)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderStyle

• `Optional` **borderStyle**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[borderStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#borderstyle)*

*Defined in [index.d.ts:1007](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1007)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### borderWidth

• `Optional` **borderWidth**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[borderWidth](_index_d_._plugin_.themabledecorationrenderoptions.md#borderwidth)*

*Defined in [index.d.ts:1013](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1013)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

___

### color

• `Optional` **color**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[color](_index_d_._plugin_.themabledecorationrenderoptions.md#color)*

*Defined in [index.d.ts:1038](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1038)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### cursor

• `Optional` **cursor**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[cursor](_index_d_._plugin_.themabledecorationrenderoptions.md#cursor)*

*Defined in [index.d.ts:1033](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1033)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### dark

• `Optional` **dark**: [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md)

*Defined in [index.d.ts:1159](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1159)*

Overwrite options for dark themes.

___

### fontStyle

• `Optional` **fontStyle**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[fontStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#fontstyle)*

*Defined in [index.d.ts:1018](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1018)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### fontWeight

• `Optional` **fontWeight**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[fontWeight](_index_d_._plugin_.themabledecorationrenderoptions.md#fontweight)*

*Defined in [index.d.ts:1023](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1023)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### gutterIconPath

• `Optional` **gutterIconPath**: string \| [Uri](../classes/_index_d_._plugin_.uri.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[gutterIconPath](_index_d_._plugin_.themabledecorationrenderoptions.md#guttericonpath)*

*Defined in [index.d.ts:1053](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1053)*

An **absolute path** or an URI to an image to be rendered in the gutter.

___

### gutterIconSize

• `Optional` **gutterIconSize**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[gutterIconSize](_index_d_._plugin_.themabledecorationrenderoptions.md#guttericonsize)*

*Defined in [index.d.ts:1060](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1060)*

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

___

### isWholeLine

• `Optional` **isWholeLine**: boolean

*Defined in [index.d.ts:1138](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1138)*

Should the decoration be rendered also on the whitespace after the line text.
Defaults to `false`.

___

### letterSpacing

• `Optional` **letterSpacing**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[letterSpacing](_index_d_._plugin_.themabledecorationrenderoptions.md#letterspacing)*

*Defined in [index.d.ts:1048](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1048)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### light

• `Optional` **light**: [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md)

*Defined in [index.d.ts:1154](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1154)*

Overwrite options for light themes.

___

### opacity

• `Optional` **opacity**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[opacity](_index_d_._plugin_.themabledecorationrenderoptions.md#opacity)*

*Defined in [index.d.ts:1043](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1043)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### outline

• `Optional` **outline**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[outline](_index_d_._plugin_.themabledecorationrenderoptions.md#outline)*

*Defined in [index.d.ts:960](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L960)*

CSS styling property that will be applied to text enclosed by a decoration.

___

### outlineColor

• `Optional` **outlineColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[outlineColor](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinecolor)*

*Defined in [index.d.ts:966](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L966)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### outlineStyle

• `Optional` **outlineStyle**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[outlineStyle](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinestyle)*

*Defined in [index.d.ts:972](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L972)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### outlineWidth

• `Optional` **outlineWidth**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[outlineWidth](_index_d_._plugin_.themabledecorationrenderoptions.md#outlinewidth)*

*Defined in [index.d.ts:978](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L978)*

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: string \| [ThemeColor](../classes/_index_d_._plugin_.themecolor.md)

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[overviewRulerColor](_index_d_._plugin_.themabledecorationrenderoptions.md#overviewrulercolor)*

*Defined in [index.d.ts:1065](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1065)*

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

___

### overviewRulerLane

• `Optional` **overviewRulerLane**: [OverviewRulerLane](../enums/_index_d_._plugin_.overviewrulerlane.md)

*Defined in [index.d.ts:1149](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1149)*

The position in the overview ruler where the decoration should be rendered.

___

### rangeBehavior

• `Optional` **rangeBehavior**: [DecorationRangeBehavior](../enums/_index_d_._plugin_.decorationrangebehavior.md)

*Defined in [index.d.ts:1144](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1144)*

Customize the growing behavior of the decoration when edits occur at the edges of the decoration's range.
Defaults to `DecorationRangeBehavior.OpenOpen`.

___

### textDecoration

• `Optional` **textDecoration**: string

*Inherited from [ThemableDecorationRenderOptions](_index_d_._plugin_.themabledecorationrenderoptions.md).[textDecoration](_index_d_._plugin_.themabledecorationrenderoptions.md#textdecoration)*

*Defined in [index.d.ts:1028](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1028)*

CSS styling property that will be applied to text enclosed by a decoration.
