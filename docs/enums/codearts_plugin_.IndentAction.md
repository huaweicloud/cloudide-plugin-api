[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / IndentAction

# Enumeration: IndentAction

["@codearts/plugin"](../modules/_codearts_plugin_.md).IndentAction

Describes what to do with the indentation when pressing Enter.

## Table of contents

### Enumeration Members

- [Indent](codearts_plugin_.IndentAction.md#indent)
- [IndentOutdent](codearts_plugin_.IndentAction.md#indentoutdent)
- [None](codearts_plugin_.IndentAction.md#none)
- [Outdent](codearts_plugin_.IndentAction.md#outdent)

## Enumeration Members

### Indent

• **Indent** = ``1``

Insert new line and indent once (relative to the previous line's indentation).

#### Defined in

[index.d.ts:5494](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5494)

___

### IndentOutdent

• **IndentOutdent** = ``2``

Insert two new lines:
 - the first one indented which will hold the cursor
 - the second one at the same indentation level

#### Defined in

[index.d.ts:5500](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5500)

___

### None

• **None** = ``0``

Insert new line and copy the previous line's indentation.

#### Defined in

[index.d.ts:5490](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5490)

___

### Outdent

• **Outdent** = ``3``

Insert new line and outdent once (relative to the previous line's indentation).

#### Defined in

[index.d.ts:5504](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5504)
