[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / DocumentLink

# Class: DocumentLink

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).DocumentLink

A document link is a range in a text document that links to an internal or external resource, like another
text document or a web site.

## Table of contents

### Constructors

- [constructor](cloudide_plugin_.DocumentLink.md#constructor)

### Properties

- [range](cloudide_plugin_.DocumentLink.md#range)
- [target](cloudide_plugin_.DocumentLink.md#target)
- [tooltip](cloudide_plugin_.DocumentLink.md#tooltip)

## Constructors

### constructor

• **new DocumentLink**(`range`, `target?`)

Creates a new document link.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](cloudide_plugin_.Range.md) | The range the document link applies to. Must not be empty. |
| `target?` | [`Uri`](cloudide_plugin_.Uri.md) | The uri the document link points to. |

#### Defined in

[index.d.ts:8470](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8470)

## Properties

### range

• **range**: [`Range`](cloudide_plugin_.Range.md)

The range this link applies to.

#### Defined in

[index.d.ts:8448](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8448)

___

### target

• `Optional` **target**: [`Uri`](cloudide_plugin_.Uri.md)

The uri this link points to.

#### Defined in

[index.d.ts:8453](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8453)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on how to
trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary depending on OS,
user settings, and localization.

#### Defined in

[index.d.ts:8462](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8462)
