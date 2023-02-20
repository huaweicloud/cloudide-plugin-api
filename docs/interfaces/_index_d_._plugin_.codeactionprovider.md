**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionProvider

# Interface: CodeActionProvider\<T>

The code action interface defines the contract between extensions and
the [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) feature.

A code action can be any command that is [known](#commands.getCommands) to the system.

## Type parameters

Name | Type | Default |
------ | ------ | ------ |
`T` | [CodeAction](../classes/_index_d_._plugin_.codeaction.md) | CodeAction |

## Hierarchy

* **CodeActionProvider**

## Index

### Methods

* [provideCodeActions](_index_d_._plugin_.codeactionprovider.md#providecodeactions)
* [resolveCodeAction](_index_d_._plugin_.codeactionprovider.md#resolvecodeaction)

## Methods

### provideCodeActions

▸ **provideCodeActions**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `range`: [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md), `context`: [CodeActionContext](_index_d_._plugin_.codeactioncontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<([Command](_index_d_._plugin_.command.md) \| [CodeAction](../classes/_index_d_._plugin_.codeaction.md))[]>

*Defined in [index.d.ts:2398](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2398)*

Provide commands for the given document and range.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](_index_d_._plugin_.textdocument.md) | The document in which the command was invoked. |
`range` | [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md) | The selector or range for which the command was invoked. This will always be a selection if there is a currently active editor. |
`context` | [CodeActionContext](_index_d_._plugin_.codeactioncontext.md) | Context carrying additional information. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<([Command](_index_d_._plugin_.command.md) \| [CodeAction](../classes/_index_d_._plugin_.codeaction.md))[]>

An array of commands, quick fixes, or refactorings or a thenable of such. The lack of a result can be
signaled by returning `undefined`, `null`, or an empty array.

___

### resolveCodeAction

▸ `Optional`**resolveCodeAction**(`codeAction`: T, `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

*Defined in [index.d.ts:2414](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L2414)*

Given a code action fill in its [`edit`](#CodeAction.edit)-property. Changes to
all other properties, like title, are ignored. A code action that has an edit
will not be resolved.

*Note* that a code action provider that returns commands, not code actions, cannot successfully
implement this function. Returning commands is deprecated and instead code actions should be
returned.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`codeAction` | T | A code action. |
`token` | [CancellationToken](_index_d_._plugin_.cancellationtoken.md) | A cancellation token. |

**Returns:** [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<T>

The resolved code action or a thenable that resolves to such. It is OK to return the given
`item`. When no result is returned, the given `item` will be used.
