[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / CodeActionProvider

# Interface: CodeActionProvider

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).CodeActionProvider

The code action interface defines the contract between extensions and
the [light bulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) feature.

A code action can be any command that is [known](#commands.getCommands) to the system.

## Table of contents

### Methods

- [provideCodeActions](cloudide_plugin_.CodeActionProvider.md#providecodeactions)

## Methods

### provideCodeActions

▸ **provideCodeActions**(`document`, `range`, `context`, `token`): [`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<([`Command`](cloudide_plugin_.Command.md) \| [`CodeAction`](../classes/cloudide_plugin_.CodeAction.md))[]\>

Provide commands for the given document and range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](cloudide_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `range` | [`Range`](../classes/cloudide_plugin_.Range.md) \| [`Selection`](../classes/cloudide_plugin_.Selection.md) | The selector or range for which the command was invoked. This will always be a selection if there is a currently active editor. |
| `context` | [`CodeActionContext`](cloudide_plugin_.CodeActionContext.md) | Context carrying additional information. |
| `token` | `undefined` \| [`CancellationToken`](cloudide_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_cloudide_plugin_.md#providerresult)<([`Command`](cloudide_plugin_.Command.md) \| [`CodeAction`](../classes/cloudide_plugin_.CodeAction.md))[]\>

An array of commands, quick fixes, or refactorings or a thenable of such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

#### Defined in

[index.d.ts:7989](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L7989)
