[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestItem

# Interface: TestItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestItem

An item shown in the "test explorer" view.

A `TestItem` can represent either a test suite or a test itself, since
they both have similar capabilities.

## Table of contents

### Properties

- [busy](codearts_plugin_.TestItem.md#busy)
- [canResolveChildren](codearts_plugin_.TestItem.md#canresolvechildren)
- [children](codearts_plugin_.TestItem.md#children)
- [description](codearts_plugin_.TestItem.md#description)
- [error](codearts_plugin_.TestItem.md#error)
- [id](codearts_plugin_.TestItem.md#id)
- [label](codearts_plugin_.TestItem.md#label)
- [parent](codearts_plugin_.TestItem.md#parent)
- [range](codearts_plugin_.TestItem.md#range)
- [sortText](codearts_plugin_.TestItem.md#sorttext)
- [tags](codearts_plugin_.TestItem.md#tags)
- [uri](codearts_plugin_.TestItem.md#uri)

## Properties

### busy

• **busy**: `boolean`

Controls whether the item is shown as "busy" in the Test Explorer view.
This is useful for showing status while discovering children.

Defaults to `false`.

#### Defined in

[index.d.ts:16209](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16209)

___

### canResolveChildren

• **canResolveChildren**: `boolean`

Indicates whether this test item may have children discovered by resolving.

If true, this item is shown as expandable in the Test Explorer view and
expanding the item will cause [resolveHandler](codearts_plugin_.TestController.md#resolvehandler)
to be invoked with the item.

Default to `false`.

#### Defined in

[index.d.ts:16201](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16201)

___

### children

• `Readonly` **children**: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)

The children of this test item. For a test suite, this may contain the
individual test cases or nested suites.

#### Defined in

[index.d.ts:16177](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16177)

___

### description

• `Optional` **description**: `string`

Optional description that appears next to the label.

#### Defined in

[index.d.ts:16219](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16219)

___

### error

• **error**: `undefined` \| `string` \| [`MarkdownString`](../classes/codearts_plugin_.MarkdownString.md)

Optional error encountered while loading the test.

Note that this is not a test result and should only be used to represent errors in
test discovery, such as syntax errors.

#### Defined in

[index.d.ts:16241](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16241)

___

### id

• `Readonly` **id**: `string`

Identifier for the `TestItem`. This is used to correlate
test results and tests in the document with those in the workspace
(test explorer). This cannot change for the lifetime of the `TestItem`,
and must be unique among its parent's direct children.

#### Defined in

[index.d.ts:16166](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16166)

___

### label

• **label**: `string`

Display name describing the test case.

#### Defined in

[index.d.ts:16214](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16214)

___

### parent

• `Readonly` **parent**: `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)

The parent of this item. It's set automatically, and is undefined
top-level items in the [items](codearts_plugin_.TestController.md#items) and for items that
aren't yet included in another item's [children](codearts_plugin_.TestItem.md#children).

#### Defined in

[index.d.ts:16184](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16184)

___

### range

• **range**: `undefined` \| [`Range`](../classes/codearts_plugin_.Range.md)

Location of the test item in its [uri](codearts_plugin_.TestItem.md#uri).

This is only meaningful if the `uri` points to a file.

#### Defined in

[index.d.ts:16233](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16233)

___

### sortText

• `Optional` **sortText**: `string`

A string that should be used when comparing this item
with other items. When `falsy` the [label](codearts_plugin_.TestItem.md#label)
is used.

#### Defined in

[index.d.ts:16226](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16226)

___

### tags

• **tags**: readonly [`TestTag`](../classes/codearts_plugin_.TestTag.md)[]

Tags associated with this test item. May be used in combination with
TestRunProfile.tags, or simply as an organizational feature.

#### Defined in

[index.d.ts:16190](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16190)

___

### uri

• `Readonly` **uri**: `undefined` \| [`Uri`](../classes/codearts_plugin_.Uri.md)

URI this `TestItem` is associated with. May be a file or directory.

#### Defined in

[index.d.ts:16171](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L16171)
