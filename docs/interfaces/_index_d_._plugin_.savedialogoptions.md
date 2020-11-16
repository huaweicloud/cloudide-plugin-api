**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / SaveDialogOptions

# Interface: SaveDialogOptions

Options to configure the behaviour of a file save dialog.

## Hierarchy

* **SaveDialogOptions**

## Index

### Properties

* [defaultUri](_index_d_._plugin_.savedialogoptions.md#defaulturi)
* [filters](_index_d_._plugin_.savedialogoptions.md#filters)
* [saveLabel](_index_d_._plugin_.savedialogoptions.md#savelabel)

## Properties

### defaultUri

• `Optional` **defaultUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1750](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1750)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1767](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1767)*

A set of file filters that are used by the dialog. Each entry is a human-readable label,
like "TypeScript", and an array of extensions, e.g.
```ts
{
	'Images': ['png', 'jpg']
	'TypeScript': ['ts', 'tsx']
}
```

___

### saveLabel

• `Optional` **saveLabel**: string

*Defined in [index.d.ts:1755](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L1755)*

A human-readable string for the save button.
