[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / TextDocumentSaveReason

# Enumeration: TextDocumentSaveReason

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).TextDocumentSaveReason

Represents reasons why a text document is saved.

## Table of contents

### Enumeration Members

- [AfterDelay](cloudide_plugin_.TextDocumentSaveReason.md#afterdelay)
- [FocusOut](cloudide_plugin_.TextDocumentSaveReason.md#focusout)
- [Manual](cloudide_plugin_.TextDocumentSaveReason.md#manual)

## Enumeration Members

### AfterDelay

• **AfterDelay** = ``2``

Automatic after a delay.

#### Defined in

[index.d.ts:1628](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1628)

___

### FocusOut

• **FocusOut** = ``3``

When the editor lost focus.

#### Defined in

[index.d.ts:1633](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1633)

___

### Manual

• **Manual** = ``1``

Manually triggered, e.g. by the user pressing save, by starting debugging,
or by an API call.

#### Defined in

[index.d.ts:1623](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L1623)
