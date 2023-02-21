[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / IndentAction

# Enumeration: IndentAction

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).IndentAction

Describes what to do with the indentation when pressing Enter.

## Table of contents

### Enumeration Members

- [Indent](cloudide_plugin_.IndentAction.md#indent)
- [IndentOutdent](cloudide_plugin_.IndentAction.md#indentoutdent)
- [None](cloudide_plugin_.IndentAction.md#none)
- [Outdent](cloudide_plugin_.IndentAction.md#outdent)

## Enumeration Members

### Indent

• **Indent** = ``1``

Insert new line and indent once (relative to the previous line's indentation).

#### Defined in

[index.d.ts:6612](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6612)

___

### IndentOutdent

• **IndentOutdent** = ``2``

Insert two new lines:
 - the first one indented which will hold the cursor
 - the second one at the same indentation level

#### Defined in

[index.d.ts:6618](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6618)

___

### None

• **None** = ``0``

Insert new line and copy the previous line's indentation.

#### Defined in

[index.d.ts:6608](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6608)

___

### Outdent

• **Outdent** = ``3``

Insert new line and outdent once (relative to the previous line's indentation).

#### Defined in

[index.d.ts:6622](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6622)
