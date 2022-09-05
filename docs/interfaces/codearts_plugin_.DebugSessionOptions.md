[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DebugSessionOptions

# Interface: DebugSessionOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).DebugSessionOptions

Options for [starting a debug session](../modules/codearts_plugin_.debug.md#startdebugging).

## Table of contents

### Properties

- [compact](codearts_plugin_.DebugSessionOptions.md#compact)
- [consoleMode](codearts_plugin_.DebugSessionOptions.md#consolemode)
- [lifecycleManagedByParent](codearts_plugin_.DebugSessionOptions.md#lifecyclemanagedbyparent)
- [noDebug](codearts_plugin_.DebugSessionOptions.md#nodebug)
- [parentSession](codearts_plugin_.DebugSessionOptions.md#parentsession)

## Properties

### compact

• `Optional` **compact**: `boolean`

Controls if the debug session's parent session is shown in the CALL STACK view even if it has only a single child.
By default, the debug session will never hide its parent.
If compact is true, debug sessions with a single child are hidden in the CALL STACK view to make the tree more compact.

#### Defined in

[index.d.ts:14597](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14597)

___

### consoleMode

• `Optional` **consoleMode**: [`DebugConsoleMode`](../enums/codearts_plugin_.DebugConsoleMode.md)

Controls whether this session should have a separate debug console or share it
with the parent session. Has no effect for sessions which do not have a parent session.
Defaults to Separate.

#### Defined in

[index.d.ts:14584](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14584)

___

### lifecycleManagedByParent

• `Optional` **lifecycleManagedByParent**: `boolean`

Controls whether lifecycle requests like 'restart' are sent to the newly created session or its parent session.
By default (if the property is false or missing), lifecycle requests are sent to the new session.
This property is ignored if the session has no parent session.

#### Defined in

[index.d.ts:14577](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14577)

___

### noDebug

• `Optional` **noDebug**: `boolean`

Controls whether this session should run without debugging, thus ignoring breakpoints.
When this property is not specified, the value from the parent session (if there is one) is used.

#### Defined in

[index.d.ts:14590](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14590)

___

### parentSession

• `Optional` **parentSession**: [`DebugSession`](codearts_plugin_.DebugSession.md)

When specified the newly created debug session is registered as a "child" session of this
"parent" debug session.

#### Defined in

[index.d.ts:14570](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L14570)
