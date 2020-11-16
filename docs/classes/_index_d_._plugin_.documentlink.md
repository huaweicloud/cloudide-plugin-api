**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DocumentLink

# Class: DocumentLink

A document link is a range in a text document that links to an internal or external resource, like another
text document or a web site.

## Hierarchy

* **DocumentLink**

## Index

### Constructors

* [constructor](_index_d_._plugin_.documentlink.md#constructor)

### Properties

* [range](_index_d_._plugin_.documentlink.md#range)
* [target](_index_d_._plugin_.documentlink.md#target)
* [tooltip](_index_d_._plugin_.documentlink.md#tooltip)

## Constructors

### constructor

\+ **new DocumentLink**(`range`: [Range](_index_d_._plugin_.range.md), `target?`: [Uri](_index_d_._plugin_.uri.md)): [DocumentLink](_index_d_._plugin_.documentlink.md)

*Defined in [index.d.ts:3999](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3999)*

Creates a new document link.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`range` | [Range](_index_d_._plugin_.range.md) | The range the document link applies to. Must not be empty. |
`target?` | [Uri](_index_d_._plugin_.uri.md) | The uri the document link points to.  |

**Returns:** [DocumentLink](_index_d_._plugin_.documentlink.md)

## Properties

### range

•  **range**: [Range](_index_d_._plugin_.range.md)

*Defined in [index.d.ts:3985](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3985)*

The range this link applies to.

___

### target

• `Optional` **target**: [Uri](_index_d_._plugin_.uri.md)

*Defined in [index.d.ts:3990](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3990)*

The uri this link points to.

___

### tooltip

• `Optional` **tooltip**: string

*Defined in [index.d.ts:3999](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L3999)*

The tooltip text when you hover over this link.

If a tooltip is provided, is will be displayed in a string that includes instructions on how to
trigger the link, such as `{0} (ctrl + click)`. The specific instructions vary depending on OS,
user settings, and localization.
