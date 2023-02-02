[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TextDocumentSaveReason

# Enumeration: TextDocumentSaveReason

["@codearts/plugin"](../modules/_codearts_plugin_.md).TextDocumentSaveReason

Represents reasons why a text document is saved.

## Table of contents

### Enumeration Members

- [AfterDelay](codearts_plugin_.TextDocumentSaveReason.md#afterdelay)
- [FocusOut](codearts_plugin_.TextDocumentSaveReason.md#focusout)
- [Manual](codearts_plugin_.TextDocumentSaveReason.md#manual)

## Enumeration Members

### AfterDelay

• **AfterDelay** = ``2``

Automatic after a delay.

#### Defined in

[index.d.ts:11674](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11674)

___

### FocusOut

• **FocusOut** = ``3``

When the editor lost focus.

#### Defined in

[index.d.ts:11679](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11679)

___

### Manual

• **Manual** = ``1``

Manually triggered, e.g. by the user pressing save, by starting debugging,
or by an API call.

#### Defined in

[index.d.ts:11669](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L11669)
