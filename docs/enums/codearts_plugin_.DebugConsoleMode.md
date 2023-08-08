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

[index.d.ts:15436](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15436)

___

### Separate

• **Separate** = ``0``

Debug session should have a separate debug console.

#### Defined in

[index.d.ts:15430](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L15430)
