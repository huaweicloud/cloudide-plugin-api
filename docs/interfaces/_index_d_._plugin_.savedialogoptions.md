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
* [title](_index_d_._plugin_.savedialogoptions.md#title)

## Properties

### defaultUri

• `Optional` **defaultUri**: [Uri](../classes/_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:1895](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1895)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1912](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1912)*

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

*Defined in [index.d.ts:1900](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1900)*

A human-readable string for the save button.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:1920](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L1920)*

Dialog title.

This parameter might be ignored, as not all operating systems display a title on save dialogs
(for example, macOS).
