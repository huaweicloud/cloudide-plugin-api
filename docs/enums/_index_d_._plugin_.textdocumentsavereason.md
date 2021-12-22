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

*Defined in [index.d.ts:10033](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10033)*

Automatic after a delay.

___

### FocusOut

•  **FocusOut**:  = 3

*Defined in [index.d.ts:10038](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10038)*

When the editor lost focus.

___

### Manual

•  **Manual**:  = 1

*Defined in [index.d.ts:10028](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10028)*

Manually triggered, e.g. by the user pressing save, by starting debugging,
or by an API call.
