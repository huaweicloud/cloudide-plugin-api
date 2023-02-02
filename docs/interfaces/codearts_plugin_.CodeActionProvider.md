[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeActionProvider

# Interface: CodeActionProvider<T\>

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeActionProvider

The code action interface defines the contract between extensions and
the [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) feature.

A code action can be any command that is [known](../modules/codearts_plugin_.commands.md#getcommands) to the system.

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`CodeAction`](../classes/codearts_plugin_.CodeAction.md) = [`CodeAction`](../classes/codearts_plugin_.CodeAction.md) |

## Table of contents

### Methods

- [provideCodeActions](codearts_plugin_.CodeActionProvider.md#providecodeactions)
- [resolveCodeAction](codearts_plugin_.CodeActionProvider.md#resolvecodeaction)

## Methods

### provideCodeActions

▸ **provideCodeActions**(`document`, `range`, `context`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<([`Command`](codearts_plugin_.Command.md) \| `T`)[]\>

Provide commands for the given document and range.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](codearts_plugin_.TextDocument.md) | The document in which the command was invoked. |
| `range` | [`Range`](../classes/codearts_plugin_.Range.md) \| [`Selection`](../classes/codearts_plugin_.Selection.md) | The selector or range for which the command was invoked. This will always be a selection if there is a currently active editor. |
| `context` | [`CodeActionContext`](codearts_plugin_.CodeActionContext.md) | Context carrying additional information. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<([`Command`](codearts_plugin_.Command.md) \| `T`)[]\>

An array of code actions, such as quick fixes or refactorings. The lack of a result can be signaled
by returning `undefined`, `null`, or an empty array.

We also support returning `Command` for legacy reasons, however all new extensions should return
`CodeAction` object instead.

#### Defined in

[index.d.ts:2502](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2502)

___

### resolveCodeAction

▸ `Optional` **resolveCodeAction**(`codeAction`, `token`): [`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

Given a code action fill in its [`edit`](../classes/codearts_plugin_.CodeAction.md#edit)-property. Changes to
all other properties, like title, are ignored. A code action that has an edit
will not be resolved.

*Note* that a code action provider that returns commands, not code actions, cannot successfully
implement this function. Returning commands is deprecated and instead code actions should be
returned.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `codeAction` | `T` | A code action. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | A cancellation token. |

#### Returns

[`ProviderResult`](../modules/_codearts_plugin_.md#providerresult)<`T`\>

The resolved code action or a thenable that resolves to such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.

#### Defined in

[index.d.ts:2518](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L2518)
