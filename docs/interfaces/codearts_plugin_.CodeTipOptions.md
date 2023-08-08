[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeTipOptions

# Interface: CodeTipOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeTipOptions

Represents options for [showCodeTip](../modules/codearts_plugin_.window.md#showcodetip)

## Table of contents

### Properties

- [severity](codearts_plugin_.CodeTipOptions.md#severity)
- [showTime](codearts_plugin_.CodeTipOptions.md#showtime)

## Properties

### severity

• `Optional` **severity**: [`CodeTipSeverity`](../enums/codearts_plugin_.CodeTipSeverity.md)

The severity of the message. Default to [Info](../enums/codearts_plugin_.CodeTipSeverity.md#info)

#### Defined in

[index.d.ts:17965](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17965)

___

### showTime

• `Optional` **showTime**: `number`

Show time(millisecond). Default to 3000. Set to -1 to always show the tip till hide event is triggered.

#### Defined in

[index.d.ts:17970](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L17970)
