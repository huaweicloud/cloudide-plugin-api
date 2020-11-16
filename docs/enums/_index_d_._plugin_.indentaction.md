**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / IndentAction

# Enumeration: IndentAction

Describes what to do with the indentation when pressing Enter.

## Index

### Enumeration members

* [Indent](_index_d_._plugin_.indentaction.md#indent)
* [IndentOutdent](_index_d_._plugin_.indentaction.md#indentoutdent)
* [None](_index_d_._plugin_.indentaction.md#none)
* [Outdent](_index_d_._plugin_.indentaction.md#outdent)

## Enumeration members

### Indent

•  **Indent**:  = 1

*Defined in [index.d.ts:4485](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4485)*

Insert new line and indent once (relative to the previous line's indentation).

___

### IndentOutdent

•  **IndentOutdent**:  = 2

*Defined in [index.d.ts:4491](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4491)*

Insert two new lines:
 - the first one indented which will hold the cursor
 - the second one at the same indentation level

___

### None

•  **None**:  = 0

*Defined in [index.d.ts:4481](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4481)*

Insert new line and copy the previous line's indentation.

___

### Outdent

•  **Outdent**:  = 3

*Defined in [index.d.ts:4495](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4495)*

Insert new line and outdent once (relative to the previous line's indentation).
