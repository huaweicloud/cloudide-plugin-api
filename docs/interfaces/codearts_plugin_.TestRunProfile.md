[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / TestRunProfile

# Interface: TestRunProfile

["@codearts/plugin"](../modules/_codearts_plugin_.md).TestRunProfile

A TestRunProfile describes one way to execute tests in a [TestController](codearts_plugin_.TestController.md).

## Table of contents

### Properties

- [configureHandler](codearts_plugin_.TestRunProfile.md#configurehandler)
- [isDefault](codearts_plugin_.TestRunProfile.md#isdefault)
- [kind](codearts_plugin_.TestRunProfile.md#kind)
- [label](codearts_plugin_.TestRunProfile.md#label)
- [runHandler](codearts_plugin_.TestRunProfile.md#runhandler)
- [tag](codearts_plugin_.TestRunProfile.md#tag)

### Methods

- [dispose](codearts_plugin_.TestRunProfile.md#dispose)

## Properties

### configureHandler

• **configureHandler**: `undefined` \| () => `void`

If this method is present, a configuration gear will be present in the
UI, and this method will be invoked when it's clicked. When called,
you can take other editor actions, such as showing a quick pick or
opening a configuration file.

#### Defined in

[index.d.ts:16381](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16381)

___

### isDefault

• **isDefault**: `boolean`

Controls whether this profile is the default action that will
be taken when its kind is actioned. For example, if the user clicks
the generic "run all" button, then the default profile for
[Run](../enums/codearts_plugin_.TestRunProfileKind.md#run) will be executed, although the
user can configure this.

#### Defined in

[index.d.ts:16367](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16367)

___

### kind

• `Readonly` **kind**: [`TestRunProfileKind`](../enums/codearts_plugin_.TestRunProfileKind.md)

Configures what kind of execution this profile controls. If there
are no profiles for a kind, it will not be available in the UI.

#### Defined in

[index.d.ts:16358](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16358)

___

### label

• **label**: `string`

Label shown to the user in the UI.

Note that the label has some significance if the user requests that
tests be re-run in a certain way. For example, if tests were run
normally and the user requests to re-run them in debug mode, the editor
will attempt use a configuration with the same label of the `Debug`
kind. If there is no such configuration, the default will be used.

#### Defined in

[index.d.ts:16352](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16352)

___

### runHandler

• **runHandler**: (`request`: [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md), `token`: [`CancellationToken`](codearts_plugin_.CancellationToken.md)) => `void` \| [`Thenable`](Thenable.md)<`void`\>

#### Type declaration

▸ (`request`, `token`): `void` \| [`Thenable`](Thenable.md)<`void`\>

Handler called to start a test run. When invoked, the function should call
[createTestRun](codearts_plugin_.TestController.md#createtestrun) at least once, and all test runs
associated with the request should be created before the function returns
or the returned promise is resolved.

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `request` | [`TestRunRequest`](../classes/codearts_plugin_.TestRunRequest.md) | Request information for the test run. |
| `token` | [`CancellationToken`](codearts_plugin_.CancellationToken.md) | - |

##### Returns

`void` \| [`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:16395](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16395)

___

### tag

• **tag**: `undefined` \| [`TestTag`](../classes/codearts_plugin_.TestTag.md)

Associated tag for the profile. If this is set, only [TestItem](codearts_plugin_.TestItem.md)
instances with the same tag will be eligible to execute in this profile.

#### Defined in

[index.d.ts:16373](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16373)

## Methods

### dispose

▸ **dispose**(): `void`

Deletes the run profile.

#### Returns

`void`

#### Defined in

[index.d.ts:16400](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16400)
