[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / BuildProfile

# Interface: BuildProfile

["@codearts/plugin"](../modules/_codearts_plugin_.md).BuildProfile

## Table of contents

### Properties

- [buildHandler](codearts_plugin_.BuildProfile.md#buildhandler)
- [configureHandler](codearts_plugin_.BuildProfile.md#configurehandler)
- [isDefault](codearts_plugin_.BuildProfile.md#isdefault)
- [label](codearts_plugin_.BuildProfile.md#label)
- [run](codearts_plugin_.BuildProfile.md#run)
- [toggleBuildStatus](codearts_plugin_.BuildProfile.md#togglebuildstatus)

### Methods

- [dispose](codearts_plugin_.BuildProfile.md#dispose)

## Properties

### buildHandler

• **buildHandler**: (`request`: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)) => `void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

#### Type declaration

▸ (`request`): `void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

Handler called to start a build run.
This function returns a method that is Thenable.
When the result is not yet returned, the build program is in a suspending state.
When it returns true or undefined, it refreshes the build status.
When it returns false, it does not change build the status.

##### Parameters

| Name | Type |
| :------ | :------ |
| `request` | [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md) |

##### Returns

`void` \| [`Thenable`](Thenable.md)<`boolean` \| `void`\>

#### Defined in

[index.d.ts:16887](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16887)

___

### configureHandler

• **configureHandler**: `undefined` \| () => `void`

If this method is present, a configuration gear will be present in the
UI, and this method will be invoked when it's clicked. When called,
you can take other editor actions, such as showing a quick pick or
opening a configuration file.

#### Defined in

[index.d.ts:16878](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16878)

___

### isDefault

• **isDefault**: `boolean`

Controls whether this profile is the default action that will
be taken when its kind is actioned. For example, if the user clicks
the generic "build" button, then the default profile will be executed,
although the user can configure this.

#### Defined in

[index.d.ts:16870](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16870)

___

### label

• **label**: `string`

Label shown to the user in the UI.

Note that the label has some significance if the user requests that
project be built in a certain way.If there is no such configuration,
the default will be used.

#### Defined in

[index.d.ts:16862](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16862)

___

### run

• **run**: (`request`: [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md)) => `void`

#### Type declaration

▸ (`request`): `void`

Execute the buildHandler that has been registered for the current profile.

##### Parameters

| Name | Type |
| :------ | :------ |
| `request` | [`BuildRequestType`](../enums/codearts_plugin_.BuildRequestType.md) |

##### Returns

`void`

#### Defined in

[index.d.ts:16892](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16892)

___

### toggleBuildStatus

• **toggleBuildStatus**: (`buildStatus`: [`BuildStatusType`](../enums/codearts_plugin_.BuildStatusType.md)) => `void`

#### Type declaration

▸ (`buildStatus`): `void`

The function is used to modify the build status corresponding to the current profile.
Developers should have sufficient understanding of this status to avoid conflicts and other issues.
At the code level, we recommend using the `profile.run` method to execute the corresponding build with the modified status
As this method is only suitable for special cases.
It has a lower priority and will not take effect when the current running build task does not belong to this profile.

##### Parameters

| Name | Type |
| :------ | :------ |
| `buildStatus` | [`BuildStatusType`](../enums/codearts_plugin_.BuildStatusType.md) |

##### Returns

`void`

#### Defined in

[index.d.ts:16901](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16901)

## Methods

### dispose

▸ **dispose**(): `void`

Deletes the build profile.

#### Returns

`void`

#### Defined in

[index.d.ts:16906](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L16906)
