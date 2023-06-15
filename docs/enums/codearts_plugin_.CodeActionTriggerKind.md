[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionTriggerKind

# Enumeration: CodeActionTriggerKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionTriggerKind

The reason why code actions were requested.

## Table of contents

### Enumeration Members

- [Automatic](codearts_plugin_.CodeActionTriggerKind.md#automatic)
- [Invoke](codearts_plugin_.CodeActionTriggerKind.md#invoke)

## Enumeration Members

### Automatic

• **Automatic** = ``2``

Code actions were requested automatically.

This typically happens when current selection in a file changes, but can
also be triggered when file content changes.

#### Defined in

[index.d.ts:2373](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2373)

___

### Invoke

• **Invoke** = ``1``

Code actions were explicitly requested by the user or by an extension.

#### Defined in

[index.d.ts:2365](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L2365)
