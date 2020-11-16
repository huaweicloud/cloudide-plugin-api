**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugSessionOptions

# Interface: DebugSessionOptions

Options for [starting a debug session](#debug.startDebugging).

## Hierarchy

* **DebugSessionOptions**

## Index

### Properties

* [consoleMode](_index_d_._plugin_.debugsessionoptions.md#consolemode)
* [parentSession](_index_d_._plugin_.debugsessionoptions.md#parentsession)

## Properties

### consoleMode

• `Optional` **consoleMode**: [DebugConsoleMode](../enums/_index_d_._plugin_.debugconsolemode.md)

*Defined in [index.d.ts:10519](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10519)*

Controls whether this session should have a separate debug console or share it
with the parent session. Has no effect for sessions which do not have a parent session.
Defaults to Separate.

___

### parentSession

• `Optional` **parentSession**: [DebugSession](_index_d_._plugin_.debugsession.md)

*Defined in [index.d.ts:10512](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L10512)*

When specified the newly created debug session is registered as a "child" session of this
"parent" debug session.
