[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ThemableDecorationRenderOptions

# Interface: ThemableDecorationRenderOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ThemableDecorationRenderOptions

Represents theme specific rendering styles for a [text editor decoration](codearts_plugin_.TextEditorDecorationType.md).

## Hierarchy

- **`ThemableDecorationRenderOptions`**

  ↳ [`DecorationRenderOptions`](codearts_plugin_.DecorationRenderOptions.md)

## Table of contents

### Properties

- [after](codearts_plugin_.ThemableDecorationRenderOptions.md#after)
- [backgroundColor](codearts_plugin_.ThemableDecorationRenderOptions.md#backgroundcolor)
- [before](codearts_plugin_.ThemableDecorationRenderOptions.md#before)
- [border](codearts_plugin_.ThemableDecorationRenderOptions.md#border)
- [borderColor](codearts_plugin_.ThemableDecorationRenderOptions.md#bordercolor)
- [borderRadius](codearts_plugin_.ThemableDecorationRenderOptions.md#borderradius)
- [borderSpacing](codearts_plugin_.ThemableDecorationRenderOptions.md#borderspacing)
- [borderStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#borderstyle)
- [borderWidth](codearts_plugin_.ThemableDecorationRenderOptions.md#borderwidth)
- [color](codearts_plugin_.ThemableDecorationRenderOptions.md#color)
- [cursor](codearts_plugin_.ThemableDecorationRenderOptions.md#cursor)
- [fontStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#fontstyle)
- [fontWeight](codearts_plugin_.ThemableDecorationRenderOptions.md#fontweight)
- [gutterIconPath](codearts_plugin_.ThemableDecorationRenderOptions.md#guttericonpath)
- [gutterIconSize](codearts_plugin_.ThemableDecorationRenderOptions.md#guttericonsize)
- [letterSpacing](codearts_plugin_.ThemableDecorationRenderOptions.md#letterspacing)
- [opacity](codearts_plugin_.ThemableDecorationRenderOptions.md#opacity)
- [outline](codearts_plugin_.ThemableDecorationRenderOptions.md#outline)
- [outlineColor](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinecolor)
- [outlineStyle](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinestyle)
- [outlineWidth](codearts_plugin_.ThemableDecorationRenderOptions.md#outlinewidth)
- [overviewRulerColor](codearts_plugin_.ThemableDecorationRenderOptions.md#overviewrulercolor)
- [textDecoration](codearts_plugin_.ThemableDecorationRenderOptions.md#textdecoration)

## Properties

### after

• `Optional` **after**: [`ThemableDecorationAttachmentRenderOptions`](codearts_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted after the decorated text.

#### Defined in

[index.d.ts:1028](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1028)

___

### backgroundColor

• `Optional` **backgroundColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

Background color of the decoration. Use rgba() and define transparent background colors to play well with other decorations.
Alternatively a color from the color registry can be [referenced](../classes/codearts_plugin_.ThemeColor.md).

#### Defined in

[index.d.ts:908](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L908)

___

### before

• `Optional` **before**: [`ThemableDecorationAttachmentRenderOptions`](codearts_plugin_.ThemableDecorationAttachmentRenderOptions.md)

Defines the rendering options of the attachment that is inserted before the decorated text.

#### Defined in

[index.d.ts:1023](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1023)

___

### border

• `Optional` **border**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:936](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L936)

___

### borderColor

• `Optional` **borderColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:942](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L942)

___

### borderRadius

• `Optional` **borderRadius**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:948](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L948)

___

### borderSpacing

• `Optional` **borderSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:954](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L954)

___

### borderStyle

• `Optional` **borderStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:960](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L960)

___

### borderWidth

• `Optional` **borderWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'border' for setting one or more of the individual border properties.

#### Defined in

[index.d.ts:966](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L966)

___

### color

• `Optional` **color**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:991](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L991)

___

### cursor

• `Optional` **cursor**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:986](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L986)

___

### fontStyle

• `Optional` **fontStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:971](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L971)

___

### fontWeight

• `Optional` **fontWeight**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:976](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L976)

___

### gutterIconPath

• `Optional` **gutterIconPath**: `string` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

An **absolute path** or an URI to an image to be rendered in the gutter.

#### Defined in

[index.d.ts:1006](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1006)

___

### gutterIconSize

• `Optional` **gutterIconSize**: `string`

Specifies the size of the gutter icon.
Available values are 'auto', 'contain', 'cover' and any percentage value.
For further information: https://msdn.microsoft.com/en-us/library/jj127316(v=vs.85).aspx

#### Defined in

[index.d.ts:1013](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1013)

___

### letterSpacing

• `Optional` **letterSpacing**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:1001](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1001)

___

### opacity

• `Optional` **opacity**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:996](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L996)

___

### outline

• `Optional` **outline**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:913](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L913)

___

### outlineColor

• `Optional` **outlineColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:919](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L919)

___

### outlineStyle

• `Optional` **outlineStyle**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:925](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L925)

___

### outlineWidth

• `Optional` **outlineWidth**: `string`

CSS styling property that will be applied to text enclosed by a decoration.
Better use 'outline' for setting one or more of the individual outline properties.

#### Defined in

[index.d.ts:931](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L931)

___

### overviewRulerColor

• `Optional` **overviewRulerColor**: `string` \| [`ThemeColor`](../classes/codearts_plugin_.ThemeColor.md)

The color of the decoration in the overview ruler. Use rgba() and define transparent colors to play well with other decorations.

#### Defined in

[index.d.ts:1018](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L1018)

___

### textDecoration

• `Optional` **textDecoration**: `string`

CSS styling property that will be applied to text enclosed by a decoration.

#### Defined in

[index.d.ts:981](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L981)
