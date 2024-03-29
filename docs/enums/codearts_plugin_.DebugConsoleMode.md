[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugConsoleMode

# Enumeration: DebugConsoleMode

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugConsoleMode

Debug console mode used by debug session, see [options](../interfaces/codearts_plugin_.DebugSessionOptions.md).

## Table of contents

### Enumeration Members

- [MergeWithParent](codearts_plugin_.DebugConsoleMode.md#mergewithparent)
- [Separate](codearts_plugin_.DebugConsoleMode.md#separate)

## Enumeration Members

### MergeWithParent

• **MergeWithParent** = ``1``

Debug session should share debug console with its parent session.
This value has no effect for sessions which do not have a parent session.

#### Defined in

[index.d.ts:15465](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15465)

___

### Separate

• **Separate** = ``0``

Debug session should have a separate debug console.

#### Defined in

[index.d.ts:15459](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L15459)
