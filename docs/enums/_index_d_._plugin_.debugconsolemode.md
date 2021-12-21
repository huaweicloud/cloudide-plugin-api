**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DebugConsoleMode

# Enumeration: DebugConsoleMode

Debug console mode used by debug session, see [options](#DebugSessionOptions).

## Index

### Enumeration members

* [MergeWithParent](_index_d_._plugin_.debugconsolemode.md#mergewithparent)
* [Separate](_index_d_._plugin_.debugconsolemode.md#separate)

## Enumeration members

### MergeWithParent

•  **MergeWithParent**:  = 1

*Defined in [index.d.ts:11916](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11916)*

Debug session should share debug console with its parent session.
This value has no effect for sessions which do not have a parent session.

___

### Separate

•  **Separate**:  = 0

*Defined in [index.d.ts:11910](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L11910)*

Debug session should have a separate debug console.
