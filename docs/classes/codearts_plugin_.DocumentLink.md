[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DocumentLink

# Class: DocumentLink

["@codearts/plugin"](../modules/_codearts_plugin_.md).DocumentLink

A document link is a range in a text document that links to an internal or external resource, like another
text document or a web site.

## Table of contents

### Constructors

- [constructor](codearts_plugin_.DocumentLink.md#constructor)

### Properties

- [range](codearts_plugin_.DocumentLink.md#range)
- [target](codearts_plugin_.DocumentLink.md#target)
- [tooltip](codearts_plugin_.DocumentLink.md#tooltip)

## Constructors

### constructor

• **new DocumentLink**(`range`, `target?`)

Creates a new document link.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `range` | [`Range`](codearts_plugin_.Range.md) | The range the document link applies to. Must not be empty. |
| `target?` | [`Uri`](codearts_plugin_.Uri.md) | The uri the document link points to. |

#### Defined in

[index.d.ts:4679](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4679)

## Properties

### range

• **range**: [`Range`](codearts_plugin_.Range.md)

The range this link applies to.

#### Defined in

[index.d.ts:4657](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4657)

___

### target

• `Optional` **target**: [`Uri`](codearts_plugin_.Uri.md)

The uri this link points to.

#### Defined in

[index.d.ts:4662](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4662)

___

### tooltip

• `Optional` **tooltip**: `string`

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on how to
trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary depending on OS,
user settings, and localization.

#### Defined in

[index.d.ts:4671](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L4671)
