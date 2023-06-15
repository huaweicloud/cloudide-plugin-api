[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DecorationRenderOptions

# Interface: DecorationRenderOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).DecorationRenderOptions

Represents rendering styles for a [text editor decoration](codearts_plugin_.TextEditorDecorationType.md).

## Hierarchy

- [`ThemableDecorationRenderOptions`](codearts_plugin_.ThemableDecorationRenderOptions.md)

  ↳ **`DecorationRenderOptions`**

## Table of contents

### Properties

- [after](codearts_plugin_.DecorationRenderOptions.md#after)
- [backgroundColor](codearts_plugin_.DecorationRenderOptions.md#backgroundcolor)
- [before](codearts_plugin_.DecorationRenderOptions.md#before)
- [border](codearts_plugin_.DecorationRenderOptions.md#border)
- [borderColor](codearts_plugin_.DecorationRenderOptions.md#bordercolor)
- [borderRadius](codearts_plugin_.DecorationRenderOptions.md#borderradius)
- [borderSpacing](codearts_plugin_.DecorationRenderOptions.md#borderspacing)
- [borderStyle](codearts_plugin_.DecorationRenderOptions.md#borderstyle)
- [borderWidth](codearts_plugin_.DecorationRenderOptions.md#borderwidth)
- [color](codearts_plugin_.DecorationRenderOptions.md#color)
- [cursor](codearts_plugin_.DecorationRenderOptions.md#cursor)
- [dark](codearts_plugin_.DecorationRenderOptions.md#dark)
- [fontStyle](codearts_plugin_.DecorationRenderOptions.md#fontstyle)
- [fontWeight](codearts_plugin_.DecorationRenderOptions.md#fontweight)
- [gutterIconPath](codearts_plugin_.DecorationRenderOptions.md#guttericonpath)
- [gutterIconSize](codearts_plugin_.DecorationRenderOptions.md#guttericonsize)
- [isWholeLine](codearts_plugin_.DecorationRenderOptions.md#iswholeline)
- [letterSpacing](codearts_plugin_.DecorationRenderOptions.md#letterspacing)
- [light](codearts_plugin_.DecorationRenderOptions.md#light)
- [opacity](codearts_plugin_.DecorationRenderOptions.md#opacity)
- [outline](codearts_plugin_.DecorationRenderOptions.md#outline)
- [outlineColor](codearts_plugin_.DecorationRenderOptions.md#outlinecolor)
- [outlineStyle](codearts_plugin_.DecorationRenderOptions.md#outlinestyle)
- [outlineWidth](codearts_plugin_.DecorationRenderOptions.md#outlinewidth)
- [overviewRulerColor](codearts_plugin_.DecorationRenderOptions.md#overviewrulercolor)
- [overviewRulerLane](codearts_plugin_.DecorationRenderOptions.md#overviewrulerlane)
- [rangeBehavior](codearts_plugin_.DecorationRenderOptions.md#rangebehavior)
- [textDecoration](codearts_plugin_.DecorationRenderOptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [`ThemableDecorationAttachmentRenderOptions`](codearts_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted after the decorated text.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[after](codearts_plugin_.ThemableDecorationRenderOptions.md#after)

#### Defined in

[index.d.ts:1028](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1028)

___

### backgroundColor

• `Optional` **backgroundColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](../classes/codearts_plugin_.ThemeColor.md).

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[backgroundColor](codearts_plugin_.ThemableDecorationRenderOptions.md#backgroundcolor)

#### Defined in

[index.d.ts:908](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L908)

___

### before

• `Optional` **before**: [`ThemableDecorationAttachmentRenderOptions`](codearts_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted before the decorated text.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[before](codearts_plugin_.ThemableDecorationRenderOptions.md#before)

#### Defined in

[index.d.ts:1023](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1023)

___

### border

• `Optional` **border**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[border](codearts_plugin_.ThemableDecorationRenderOptions.md#border)

#### Defined in

[index.d.ts:936](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L936)

___

### borderColor

• `Optional` **borderColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[borderColor](codearts_plugin_.ThemableDecorationRenderOptions.md#bordercolor)

#### Defined in

[index.d.ts:942](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L942)

___

### borderRadius

• `Optional` **borderRadius**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[borderRadius](codearts_plugin_.ThemableDecorationRenderOptions.md#borderradius)

#### Defined in

[index.d.ts:948](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L948)

___

### borderSpacing

• `Optional` **borderSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[borderSpacing](codearts_plugin_.ThemableDecorationRenderOptions.md#borderspacing)

#### Defined in

[index.d.ts:954](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L954)

___

### borderStyle

• `Optional` **borderStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[borderStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#borderstyle)

#### Defined in

[index.d.ts:960](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L960)

___

### borderWidth

• `Optional` **borderWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[borderWidth](codearts_plugin_.ThemableDecorationRenderOptions.md#borderwidth)

#### Defined in

[index.d.ts:966](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L966)

___

### color

• `Optional` **color**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[color](codearts_plugin_.ThemableDecorationRenderOptions.md#color)

#### Defined in

[index.d.ts:991](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L991)

___

### cursor

• `Optional` **cursor**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[cursor](codearts_plugin_.ThemableDecorationRenderOptions.md#cursor)

#### Defined in

[index.d.ts:986](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L986)

___

### dark

• `Optional` **dark**: [`ThemableDecorationRenderOptions`](codearts_plugin_.ThemableDecorationRenderOptions.md)

Overwrite options for dark themes.

#### Defined in

[index.d.ts:1112](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1112)

___

### fontStyle

• `Optional` **fontStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[fontStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#fontstyle)

#### Defined in

[index.d.ts:971](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L971)

___

### fontWeight

• `Optional` **fontWeight**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[fontWeight](codearts_plugin_.ThemableDecorationRenderOptions.md#fontweight)

#### Defined in

[index.d.ts:976](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L976)

___

### gutterIconPath

• `Optional` **gutterIconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

An **absolute path** or an URI to an image to be rendered in the gutter.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[gutterIconPath](codearts_plugin_.ThemableDecorationRenderOptions.md#guttericonpath)

#### Defined in

[index.d.ts:1006](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1006)

___

### gutterIconSize

• `Optional` **gutterIconSize**: `string`

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[gutterIconSize](codearts_plugin_.ThemableDecorationRenderOptions.md#guttericonsize)

#### Defined in

[index.d.ts:1013](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1013)

___

### isWholeLine

• `Optional` **isWholeLine**: `boolean`

Should the decoration be rendered also on the whitespace after the line text.
Defaults to `false`.

#### Defined in

[index.d.ts:1091](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1091)

___

### letterSpacing

• `Optional` **letterSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[letterSpacing](codearts_plugin_.ThemableDecorationRenderOptions.md#letterspacing)

#### Defined in

[index.d.ts:1001](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1001)

___

### light

• `Optional` **light**: [`ThemableDecorationRenderOptions`](codearts_plugin_.ThemableDecorationRenderOptions.md)

Overwrite options for light themes.

#### Defined in

[index.d.ts:1107](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1107)

___

### opacity

• `Optional` **opacity**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[opacity](codearts_plugin_.ThemableDecorationRenderOptions.md#opacity)

#### Defined in

[index.d.ts:996](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L996)

___

### outline

• `Optional` **outline**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[outline](codearts_plugin_.ThemableDecorationRenderOptions.md#outline)

#### Defined in

[index.d.ts:913](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L913)

___

### outlineColor

• `Optional` **outlineColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[outlineColor](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinecolor)

#### Defined in

[index.d.ts:919](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L919)

___

### outlineStyle

• `Optional` **outlineStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[outlineStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinestyle)

#### Defined in

[index.d.ts:925](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L925)

___

### outlineWidth

• `Optional` **outlineWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[outlineWidth](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinewidth)

#### Defined in

[index.d.ts:931](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L931)

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[overviewRulerColor](codearts_plugin_.ThemableDecorationRenderOptions.md#overviewrulercolor)

#### Defined in

[index.d.ts:1018](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1018)

___

### overviewRulerLane

• `Optional` **overviewRulerLane**: [`OverviewRulerLane`](../enums/codearts_plugin_.OverviewRulerLane.md)

The position in the overview ruler where the decoration should be rendered.

#### Defined in

[index.d.ts:1102](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1102)

___

### rangeBehavior

• `Optional` **rangeBehavior**: [`DecorationRangeBehavior`](../enums/codearts_plugin_.DecorationRangeBehavior.md)

Customize the growing behavior of the decoration when edits occur at the edges of the decoration's range.
Defaults to `DecorationRangeBehavior.OpenOpen`.

#### Defined in

[index.d.ts:1097](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L1097)

___

### textDecoration

• `Optional` **textDecoration**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Inherited from

[ThemableDecorationRenderOptions](codearts_plugin_.ThemableDecorationRenderOptions.md).[textDecoration](codearts_plugin_.ThemableDecorationRenderOptions.md#textdecoration)

#### Defined in

[index.d.ts:981](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L981)
