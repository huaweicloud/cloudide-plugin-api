[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / QuickPickItemKind

# Enumeration: QuickPickItemKind

["@codearts/plugin"](../modules/_codearts_plugin_.md).QuickPickItemKind

The kind of [quick pick item](../interfaces/codearts_plugin_.QuickPickItem.md).

## Table of contents

### Enumeration Members

- [Default](codearts_plugin_.QuickPickItemKind.md#default)
- [Separator](codearts_plugin_.QuickPickItemKind.md#separator)

## Enumeration Members

### Default

• **Default** = ``0``

The default [kind](../interfaces/codearts_plugin_.QuickPickItem.md#kind) is an item that can be selected in the quick pick.

#### Defined in

[index.d.ts:1724](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1724)

___

### Separator

• **Separator** = ``-1``

When a [QuickPickItem](../interfaces/codearts_plugin_.QuickPickItem.md) has a kind of [Separator](codearts_plugin_.QuickPickItemKind.md#separator), the item is just a visual separator and does not represent a real item.
The only property that applies is [label](../interfaces/codearts_plugin_.QuickPickItem.md#label). All other properties on [QuickPickItem](../interfaces/codearts_plugin_.QuickPickItem.md) will be ignored and have no effect.

#### Defined in

[index.d.ts:1720](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1720)
