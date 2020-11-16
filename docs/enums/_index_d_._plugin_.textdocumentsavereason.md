**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TextDocumentSaveReason

# Enumeration: TextDocumentSaveReason

Represents reasons why a text document is saved.

## Index

### Enumeration members

* [AfterDelay](_index_d_._plugin_.textdocumentsavereason.md#afterdelay)
* [FocusOut](_index_d_._plugin_.textdocumentsavereason.md#focusout)
* [Manual](_index_d_._plugin_.textdocumentsavereason.md#manual)

## Enumeration members

### AfterDelay

•  **AfterDelay**:  = 2

*Defined in [index.d.ts:8663](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8663)*

Automatic after a delay.

___

### FocusOut

•  **FocusOut**:  = 3

*Defined in [index.d.ts:8668](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8668)*

When the editor lost focus.

___

### Manual

•  **Manual**:  = 1

*Defined in [index.d.ts:8658](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L8658)*

Manually triggered, e.g. by the user pressing save, by starting debugging,
or by an API call.
