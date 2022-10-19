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

[index.d.ts:11503](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L11503)

___

### FocusOut

• **FocusOut** = ``3``

When the editor lost focus.

#### Defined in

[index.d.ts:11508](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L11508)

___

### Manual

• **Manual** = ``1``

Manually triggered, e.g. by the user pressing save, by starting debugging,
or by an API call.

#### Defined in

[index.d.ts:11498](https://github.com/huaweicloud/cloudide-plugin-api/blob/5055bbd/index.d.ts#L11498)
