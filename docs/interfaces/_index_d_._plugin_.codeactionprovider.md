**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / CodeActionProvider

# Interface: CodeActionProvider

The code action interface defines the contract between extensions and
the [lightbulb](https://code.visualstudio.com/docs/editor/editingevolved#_code-action) feature.

A code action can be any command that is [known](#commands.getCommands) to the system.

## Hierarchy

* **CodeActionProvider**

## Index

### Methods

* [provideCodeActions](_index_d_._plugin_.codeactionprovider.md#providecodeactions)

## Methods

### provideCodeActions

▸ **provideCodeActions**(`document`: [TextDocument](_index_d_._plugin_.textdocument.md), `range`: [Range](../classes/_index_d_._plugin_.range.md) \| [Selection](../classes/_index_d_._plugin_.selection.md), `context`: [CodeActionContext](_index_d_._plugin_.codeactioncontext.md), `token`: [CancellationToken](_index_d_._plugin_.cancellationtoken.md)): [ProviderResult](../modules/_index_d_._plugin_.md#providerresult)\<([Command](_index_d_._plugin_.command.md) \| [CodeAction](../classes/_index_d_._plugin_.codeaction.md))[]>

*Defined in [index.d.ts:2223](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L2223)*

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
