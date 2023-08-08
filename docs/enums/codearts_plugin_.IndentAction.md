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

[index.d.ts:5532](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5532)

___

### IndentOutdent

• **IndentOutdent** = ``2``

Insert two new lines:
 - the first one indented which will hold the cursor
 - the second one at the same indentation level

#### Defined in

[index.d.ts:5538](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5538)

___

### None

• **None** = ``0``

Insert new line and copy the previous line's indentation.

#### Defined in

[index.d.ts:5528](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5528)

___

### Outdent

• **Outdent** = ``3``

Insert new line and outdent once (relative to the previous line's indentation).

#### Defined in

[index.d.ts:5542](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5542)
