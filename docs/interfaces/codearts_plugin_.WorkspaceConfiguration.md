[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WorkspaceConfiguration

# Interface: WorkspaceConfiguration

["@codearts/plugin"](../modules/_codearts_plugin_.md).WorkspaceConfiguration

Represents the configuration. It is a merged view of

- *Default Settings*
- *Global (User) Settings*
- *Workspace settings*
- *Workspace Folder settings* - From one of the [Workspace Folders](../modules/codearts_plugin_.workspace.md#workspacefolders) under which requested resource belongs to.
- *Language settings* - Settings defined under requested language.

The *effective* value (returned by [`get`](codearts_plugin_.WorkspaceConfiguration.md#get)) is computed by overriding or merging the values in the following order:

1. `defaultValue` (if defined in `package.json` otherwise derived from the value's type)
1. `globalValue` (if defined)
1. `workspaceValue` (if defined)
1. `workspaceFolderValue` (if defined)
1. `defaultLanguageValue` (if defined)
1. `globalLanguageValue` (if defined)
1. `workspaceLanguageValue` (if defined)
1. `workspaceFolderLanguageValue` (if defined)

**Note:** Only `object` value types are merged and all other value types are overridden.

Example 1: Overriding

```ts
defaultValue = 'on';
globalValue = 'relative'
workspaceFolderValue = 'off'
value = 'off'
```

Example 2: Language Values

```ts
defaultValue = 'on';
globalValue = 'relative'
workspaceFolderValue = 'off'
globalLanguageValue = 'on'
value = 'on'
```

Example 3: Object Values

```ts
defaultValue = { "a": 1, "b": 2 };
globalValue = { "b": 3, "c": 4 };
value = { "a": 1, "b": 3, "c": 4 };
```

*Note:* Workspace and Workspace Folder configurations contains `launch` and `tasks` settings. Their basename will be
part of the section identifier. The following snippets shows how to retrieve all configurations
from `launch.json`:

```ts
// launch.json configuration
const config = workspace.getConfiguration('launch', vscode.workspace.workspaceFolders[0].uri);

// retrieve values
const values = config.get('configurations');
```

Refer to [Settings](https://code.visualstudio.com/docs/getstarted/settings) for more information.

## Indexable

▪ [key: `string`]: `any`

## Table of contents

### Methods

- [get](codearts_plugin_.WorkspaceConfiguration.md#get)
- [has](codearts_plugin_.WorkspaceConfiguration.md#has)
- [inspect](codearts_plugin_.WorkspaceConfiguration.md#inspect)
- [update](codearts_plugin_.WorkspaceConfiguration.md#update)

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

[index.d.ts:5709](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5709)

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

[index.d.ts:5718](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5718)

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

[index.d.ts:5726](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5726)

___

### inspect

▸ **inspect**<`T`\>(`section`): `undefined` \| { `defaultLanguageValue?`: `T` ; `defaultValue?`: `T` ; `globalLanguageValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `languageIds?`: `string`[] ; `workspaceFolderLanguageValue?`: `T` ; `workspaceFolderValue?`: `T` ; `workspaceLanguageValue?`: `T` ; `workspaceValue?`: `T`  }

Retrieve all information about a configuration setting. A configuration value
often consists of a *default* value, a global or installation-wide value,
a workspace-specific value, folder-specific value
and language-specific values (if [WorkspaceConfiguration](codearts_plugin_.WorkspaceConfiguration.md) is scoped to a language).

Also provides all language ids under which the given configuration setting is defined.

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

`undefined` \| { `defaultLanguageValue?`: `T` ; `defaultValue?`: `T` ; `globalLanguageValue?`: `T` ; `globalValue?`: `T` ; `key`: `string` ; `languageIds?`: `string`[] ; `workspaceFolderLanguageValue?`: `T` ; `workspaceFolderValue?`: `T` ; `workspaceLanguageValue?`: `T` ; `workspaceValue?`: `T`  }

Information about a configuration setting or `undefined`.

#### Defined in

[index.d.ts:5742](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5742)

___

### update

▸ **update**(`section`, `value`, `configurationTarget?`, `overrideInLanguage?`): [`Thenable`](Thenable.md)<`void`\>

Update a configuration value. The updated configuration values are persisted.

A value can be changed in

- [Global settings](../enums/codearts_plugin_.ConfigurationTarget.md#global): Changes the value for all instances of the editor.
- [Workspace settings](../enums/codearts_plugin_.ConfigurationTarget.md#workspace): Changes the value for current workspace, if available.
- [Workspace folder settings](../enums/codearts_plugin_.ConfigurationTarget.md#workspacefolder): Changes the value for settings from one of the [Workspace Folders](../modules/codearts_plugin_.workspace.md#workspacefolders) under which the requested resource belongs to.
- Language settings: Changes the value for the requested languageId.

*Note:* To remove a configuration value use `undefined`, like so: `config.update('somekey', undefined)`

**`Throws`**

error while updating
	- configuration which is not registered.
	- window configuration to workspace folder
	- configuration to workspace or workspace folder when no workspace is opened.
	- configuration to workspace folder when there is no workspace folder settings.
	- configuration to workspace folder when [WorkspaceConfiguration](codearts_plugin_.WorkspaceConfiguration.md) is not scoped to a resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `section` | `string` | Configuration name, supports _dotted_ names. |
| `value` | `any` | The new value. |
| `configurationTarget?` | ``null`` \| `boolean` \| [`ConfigurationTarget`](../enums/codearts_plugin_.ConfigurationTarget.md) | The [configuration target](../enums/codearts_plugin_.ConfigurationTarget.md) or a boolean value.  - If `true` updates [Global settings](../enums/codearts_plugin_.ConfigurationTarget.md#global).  - If `false` updates [Workspace settings](../enums/codearts_plugin_.ConfigurationTarget.md#workspace).  - If `undefined` or `null` updates to [Workspace folder settings](../enums/codearts_plugin_.ConfigurationTarget.md#workspacefolder) if configuration is resource specific,  otherwise to [Workspace settings](../enums/codearts_plugin_.ConfigurationTarget.md#workspace). |
| `overrideInLanguage?` | `boolean` | Whether to update the value in the scope of requested languageId or not.  - If `true` updates the value under the requested languageId.  - If `undefined` updates the value under the requested languageId only if the configuration is defined for the language. |

#### Returns

[`Thenable`](Thenable.md)<`void`\>

#### Defined in

[index.d.ts:5788](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L5788)
