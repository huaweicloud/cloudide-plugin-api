**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugSessionOptions

# Interface: DebugSessionOptions

Options for [starting a debug session](#debug.startDebugging).

## Hierarchy

* **DebugSessionOptions**

## Index

### Properties

* [compact](_index_d_._plugin_.debugsessionoptions.md#compact)
* [consoleMode](_index_d_._plugin_.debugsessionoptions.md#consolemode)
* [noDebug](_index_d_._plugin_.debugsessionoptions.md#nodebug)
* [parentSession](_index_d_._plugin_.debugsessionoptions.md#parentsession)

## Properties

### compact

• `Optional` **compact**: boolean

*Defined in [index.d.ts:12000](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L12000)*

Controls if the debug session's parent session is shown in the CALL STACK view even if it has only a single child.
By default, the debug session will never hide its parent.
If compact is true, debug sessions with a single child are hidden in the CALL STACK view to make the tree more compact.

___

### consoleMode

• `Optional` **consoleMode**: [DebugConsoleMode](../enums/_index_d_._plugin_.debugconsolemode.md)

*Defined in [index.d.ts:11987](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11987)*

Controls whether this session should have a separate debug console or share it
with the parent session. Has no effect for sessions which do not have a parent session.
Defaults to Separate.

___

### noDebug

• `Optional` **noDebug**: boolean

*Defined in [index.d.ts:11993](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11993)*

Controls whether this session should run without debugging, thus ignoring breakpoints.
When this property is not specified, the value from the parent session (if there is one) is used.

___

### parentSession

• `Optional` **parentSession**: [DebugSession](_index_d_._plugin_.debugsession.md)

*Defined in [index.d.ts:11980](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L11980)*

When specified the newly created debug session is registered as a "child" session of this
"parent" debug session.
