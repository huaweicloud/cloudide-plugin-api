[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / InputBoxValidationMessage

# Interface: InputBoxValidationMessage

["@codearts/plugin"](../modules/_codearts_plugin_.md).InputBoxValidationMessage

Object to configure the behavior of the validation message.

## Table of contents

### Properties

- [message](codearts_plugin_.InputBoxValidationMessage.md#message)
- [severity](codearts_plugin_.InputBoxValidationMessage.md#severity)

## Properties

### message

• `Readonly` **message**: `string`

The validation message to display.

#### Defined in

[index.d.ts:2002](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2002)

___

### severity

• `Readonly` **severity**: [`InputBoxValidationSeverity`](../enums/codearts_plugin_.InputBoxValidationSeverity.md)

The severity of the validation message.
NOTE: When using `InputBoxValidationSeverity.Error`, the user will not be allowed to accept (hit ENTER) the input.
`Info` and `Warning` will still allow the InputBox to accept the input.

#### Defined in

[index.d.ts:2009](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L2009)
