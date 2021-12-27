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

*Defined in [index.d.ts:1898](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1898)*

The resource the dialog shows when opened.

___

### filters

• `Optional` **filters**: { [name:string]: string[];  }

*Defined in [index.d.ts:1915](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1915)*

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

*Defined in [index.d.ts:1903](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1903)*

A human-readable string for the save button.

___

### title

• `Optional` **title**: string

*Defined in [index.d.ts:1923](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L1923)*

Dialog title.

This parameter might be ignored, as not all operating systems display a title on save dialogs
(for example, macOS).
