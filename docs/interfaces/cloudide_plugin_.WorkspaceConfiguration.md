[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WorkspaceConfiguration

# Interface: WorkspaceConfiguration

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WorkspaceConfiguration

Represents the configuration. It is a merged view of

- Default configuration
- Global configuration
- Workspace configuration (if available)
- Workspace folder configuration of the requested resource (if available)

*Global configuration* comes from User Settings and shadows Defaults.

*Workspace configuration* comes from Workspace Settings and shadows Global configuration.

*Workspace Folder configuration* comes from `.vscode` folder under one of the [workspace folders](#workspace.workspaceFolders).

*Note:* Workspace and Workspace Folder configurations contains `launch` and `tasks` settings. Their basename will be
part of the section identifier. The following snippets shows how to retrieve all configurations
from `launch.json`:

```ts
// launch.json configuration
const config = workspace.getConfiguration('launch', vscode.window.activeTextEditor.document.uri);

// retrieve values
const values = config.get('configurations');
```

Refer to [Settings](https://code.visualstudio.com/docs/getstarted/settings) for more information.

## Indexable

▪ [key: `string`]: `any`

## Table of contents

### Methods

- [get](cloudide_plugin_.WorkspaceConfiguration.md#get)
- [has](cloudide_plugin_.WorkspaceConfiguration.md#has)
- [inspect](cloudide_plugin_.WorkspaceConfiguration.md#inspect)
- [update](cloudide_plugin_.WorkspaceConfiguration.md#update)

## Methods

### get

▸ **get**<`T`\>(`section`): `undefined` \| `T`

Return a value from this configuration.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |

#### Returns

`undefined` \| `T`

The value `section` denotes or `undefined`.

#### Defined in

[index.d.ts:5441](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5441)

▸ **get**<`T`\>(`section`, `defaultValue`): `T`

Return a value from this configuration.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |
| `defaultValue` | `T` | A value should be returned when no value could be found, is `undefined`. |

#### Returns

`T`

The value `section` denotes or the default.

#### Defined in

[index.d.ts:5450](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5450)

___

### has

▸ **has**(`section`): `boolean`

Check if this configuration has a certain value.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |

#### Returns

`boolean`

`true` if the section doesn't resolve to `undefined`.

#### Defined in

[index.d.ts:5458](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5458)

___

### inspect

▸ **inspect**<`T`\>(`section`): `undefined` \| { `defaultValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `workspaceFolderValue?`: `T` ; `workspaceValue?`: `T`  }

Retrieve all information about a configuration setting. A configuration value
often consists of a *default* value, a global or installation-wide value,
a workspace-specific value and a folder-specific value.

The *effective* value (returned by [`get`](#WorkspaceConfiguration.get))
is computed like this: `defaultValue` overwritten by `globalValue`,
`globalValue` overwritten by `workspaceValue`. `workspaceValue` overwritten by `workspaceFolderValue`.
Refer to [Settings Inheritance](https://code.visualstudio.com/docs/getstarted/settings)
for more information.

*Note:* The configuration name must denote a leaf in the configuration tree
(`editor.fontSize` vs `editor`) otherwise no result is returned.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |

#### Returns

`undefined` \| { `defaultValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `workspaceFolderValue?`: `T` ; `workspaceValue?`: `T`  }

Information about a configuration setting or `undefined`.

#### Defined in

[index.d.ts:5477](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5477)

___

### update

▸ **update**(`section`, `value`, `configurationTarget?`): `PromiseLike`<`void`\>

Update a configuration value. The updated configuration values are persisted.

A value can be changed in

- [Global configuration](#ConfigurationTarget.Global): Changes the value for all instances of the editor.
- [Workspace configuration](#ConfigurationTarget.Workspace): Changes the value for current workspace, if available.
- [Workspace folder configuration](#ConfigurationTarget.WorkspaceFolder): Changes the value for the
[Workspace folder](#workspace.workspaceFolders) to which the current [configuration](#WorkspaceConfiguration) is scoped to.

*Note 1:* Setting a global value in the presence of a more specific workspace value
has no observable effect in that workspace, but in others. Setting a workspace value
in the presence of a more specific folder value has no observable effect for the resources
under respective [folder](#workspace.workspaceFolders), but in others. Refer to
[Settings Inheritence](https://code.visualstudio.com/docs/getstarted/settings) for more information.

*Note 2:* To remove a configuration value use `undefined`, like so: `config.update('somekey', undefined)`

Will throw error when
- Writing a configuration which is not registered.
- Writing a configuration to workspace or folder target when no workspace is opened
- Writing a configuration to folder target when there is no folder settings
- Writing to folder target without passing a resource when getting the configuration (`workspace.getConfiguration(section, resource)`)
- Writing a window configuration to folder target

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |
| `value` | `any` | The new value. |
| `configurationTarget?` | `boolean` \| [`ConfigurationTarget`](../enums/cloudide_plugin_.ConfigurationTarget.md) | The [configuration target](#ConfigurationTarget) or a boolean value. - If `true` configuration target is `ConfigurationTarget.Global`. - If `false` configuration target is `ConfigurationTarget.Workspace`. - If `undefined` or `null` configuration target is `ConfigurationTarget.WorkspaceFolder` when configuration is resource specific `ConfigurationTarget.Workspace` otherwise. |

#### Returns

`PromiseLike`<`void`\>

#### Defined in

[index.d.ts:5513](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L5513)
