[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestController

# Interface: TestController

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestController

Entry point to discover and execute tests. It contains [items](codearts_plugin_.TestController.md#items) which
are used to populate the editor UI, and is associated with
[run profiles](codearts_plugin_.TestController.md#createrunprofile) to allow
for tests to be executed.

## Table of contents

### Properties

- [id](codearts_plugin_.TestController.md#id)
- [items](codearts_plugin_.TestController.md#items)
- [label](codearts_plugin_.TestController.md#label)
- [refreshHandler](codearts_plugin_.TestController.md#refreshhandler)
- [resolveHandler](codearts_plugin_.TestController.md#resolvehandler)

### Methods

- [createRunProfile](codearts_plugin_.TestController.md#createrunprofile)
- [createTestItem](codearts_plugin_.TestController.md#createtestitem)
- [createTestRun](codearts_plugin_.TestController.md#createtestrun)
- [dispose](codearts_plugin_.TestController.md#dispose)

## Properties

### id

• `Readonly` **id**: `string`

The id of the controller passed in vscode.tests.createTestController.
This must be globally unique.

#### Defined in

[index.d.ts:16253](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16253)

___

### items

• `Readonly` **items**: [`TestItemCollection`](codearts_plugin_.TestItemCollection.md)

A collection of "top-level" [TestItem](codearts_plugin_.TestItem.md) instances, which can in
turn have their own [children](codearts_plugin_.TestItem.md#children) to form the
"test tree."

The extension controls when to add tests. For example, extensions should
add tests for a file when vscode.workspace.onDidOpenTextDocument
fires in order for decorations for tests within a file to be visible.

However, the editor may sometimes explicitly request children using the
[resolveHandler](codearts_plugin_.TestController.md#resolvehandler) See the documentation on that method for more details.

#### Defined in

[index.d.ts:16272](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16272)

___

### label

• **label**: `string`

Human-readable label for the test controller.

#### Defined in

[index.d.ts:16258](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16258)

___

### refreshHandler

• **refreshHandler**: `undefined` \| (`token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

If this method is present, a refresh button will be present in the
UI, and this method will be invoked when it's clicked. When called,
the extension should scan the workspace for any new, changed, or
removed tests.

It's recommended that extensions try to update tests in realtime, using
a [FileSystemWatcher](codearts_plugin_.FileSystemWatcher.md) for example, and use this method as a fallback.

#### Defined in

[index.d.ts:16318](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16318)

___

### resolveHandler

• `Optional` **resolveHandler**: (`item`: `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Type declaration

▸ (`item`): `void` \| [`Thenable`](Thenable.md)<`void`\>

A function provided by the extension that the editor may call to request
children of a test item, if the [canResolveChildren](codearts_plugin_.TestItem.md#canresolvechildren) is
`true`. When called, the item should discover children and call
vscode.tests.createTestItem as children are discovered.

Generally the extension manages the lifecycle of test items, but under
certain conditions the editor may request the children of a specific
item to be loaded. For example, if the user requests to re-run tests
after reloading the editor, the editor may need to call this method
to resolve the previously-run tests.

The item in the explorer will automatically be marked as "busy" until
the function returns or the returned thenable resolves.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `item` | `undefined` \| [`TestItem`](codearts_plugin_.TestItem.md) | An unresolved test item for which children are being requested, or `undefined` to resolve the controller's initial [items](codearts_plugin_.TestController.md#items). |

##### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:16305](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16305)

## Methods

### createRunProfile

▸ **createRunProfile**(`label`, `kind`, `runHandler`, `isDefault?`, `tag?`): [`TestRunProfile`](codearts_plugin_.TestRunProfile.md)

Creates a profile used for running tests. Extensions must create
at least one profile in order for tests to be run.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` | A human-readable label for this profile. |
| `kind` | [`TestRunProfileKind`](../enums/codearts_plugin_.TestRunProfileKind.md) | Configures what kind of execution this profile manages. |
| `runHandler` | (`request`: [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md), `token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\> | Function called to start a test run. |
| `isDefault?` | `boolean` | Whether this is the default action for its kind. |
| `tag?` | [`TestTag`](../classes/codearts_plugin_.TestTag.md) | Profile test tag. |

#### Returns

[`TestRunProfile`](codearts_plugin_.TestRunProfile.md)

An instance of a [TestRunProfile](codearts_plugin_.TestRunProfile.md), which is automatically
associated with this controller.

#### Defined in

[index.d.ts:16285](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16285)

___

### createTestItem

▸ **createTestItem**(`id`, `label`, `uri?`, `testItemLevel?`): [`TestItem`](codearts_plugin_.TestItem.md)

Creates a new managed [TestItem](codearts_plugin_.TestItem.md) instance. It can be added into
the [children](codearts_plugin_.TestItem.md#children) of an existing item, or into the
[items](codearts_plugin_.TestController.md#items).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | Identifier for the TestItem. The test item's ID must be unique in the [TestItemCollection](codearts_plugin_.TestItemCollection.md) it's added to. |
| `label` | `string` | Human-readable label of the test item. |
| `uri?` | [`Uri`](../classes/codearts_plugin_.Uri.md) | URI this TestItem is associated with. May be a file or directory. |
| `testItemLevel?` | `string` | the hierarchical relationship of the current TestItem. |

#### Returns

[`TestItem`](codearts_plugin_.TestItem.md)

#### Defined in

[index.d.ts:16354](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16354)

___

### createTestRun

▸ **createTestRun**(`request`, `name?`, `persist?`): [`TestRun`](codearts_plugin_.TestRun.md)

Creates a [TestRun](codearts_plugin_.TestRun.md). This should be called by the
[TestRunProfile](codearts_plugin_.TestRunProfile.md) when a request is made to execute tests, and may
also be called if a test run is detected externally. Once created, tests
that are included in the request will be moved into the queued state.

All runs created using the same `request` instance will be grouped
together. This is useful if, for example, a single suite of tests is
run on multiple platforms.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md) | Test run request. Only tests inside the `include` may be modified, and tests in its `exclude` are ignored. |
| `name?` | `string` | The human-readable name of the run. This can be used to disambiguate multiple sets of results in a test run. It is useful if tests are run across multiple platforms, for example. |
| `persist?` | `boolean` | Whether the results created by the run should be persisted in the editor. This may be false if the results are coming from a file already saved externally, such as a coverage information file. |

#### Returns

[`TestRun`](codearts_plugin_.TestRun.md)

An instance of the [TestRun](codearts_plugin_.TestRun.md). It will be considered "running"
from the moment this method is invoked until [end](codearts_plugin_.TestRun.md#end) is called.

#### Defined in

[index.d.ts:16341](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16341)

___

### dispose

▸ **dispose**(): `void`

Unregisters the test controller, disposing of its associated tests
and unpersisted results.

#### Returns

`void`

#### Defined in

[index.d.ts:16360](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L16360)
