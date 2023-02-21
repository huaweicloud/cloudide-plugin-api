[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DebugSessionOptions

# Interface: DebugSessionOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DebugSessionOptions

Options for starting a debug session.

## Table of contents

### Properties

- [compact](cloudide_plugin_.DebugSessionOptions.md#compact)
- [consoleMode](cloudide_plugin_.DebugSessionOptions.md#consolemode)
- [noDebug](cloudide_plugin_.DebugSessionOptions.md#nodebug)
- [parentSession](cloudide_plugin_.DebugSessionOptions.md#parentsession)

## Properties

### compact

• `Optional` **compact**: `boolean`

Controls if the debug session's parent session is shown in the CALL STACK view even if it has only a single child.
By default, the debug session will never hide its parent.
If compact is true, debug sessions with a single child are hidden in the CALL STACK view to make the tree more compact.

#### Defined in

[index.d.ts:9674](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9674)

___

### consoleMode

• `Optional` **consoleMode**: [`DebugConsoleMode`](../enums/cloudide_plugin_.DebugConsoleMode.md)

Controls whether this session should have a separate debug console or share it
with the parent session. Has no effect for sessions which do not have a parent session.
Defaults to Separate.

#### Defined in

[index.d.ts:9661](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9661)

___

### noDebug

• `Optional` **noDebug**: `boolean`

Controls whether this session should run without debugging, thus ignoring breakpoints.
When this property is not specified, the value from the parent session (if there is one) is used.

#### Defined in

[index.d.ts:9667](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9667)

___

### parentSession

• `Optional` **parentSession**: [`DebugSession`](cloudide_plugin_.DebugSession.md)

When specified the newly created debug session is registered as a "child" session of this
"parent" debug session.

#### Defined in

[index.d.ts:9654](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9654)
