**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WorkspaceConfiguration

# Interface: WorkspaceConfiguration

Represents the configuration. It is a merged view of

- *Default Settings*
- *Global (User) Settings*
- *Workspace settings*
- *Workspace Folder settings* - From one of the [Workspace Folders](#workspace.workspaceFolders) under which requested resource belongs to.
- *Language settings* - Settings defined under requested language.

The *effective* value (returned by [`get`](#WorkspaceConfiguration.get)) is computed by overriding or merging the values in the following order.

```
`defaultValue`
`globalValue` (if defined)
`workspaceValue` (if defined)
`workspaceFolderValue` (if defined)
`defaultLanguageValue` (if defined)
`globalLanguageValue` (if defined)
`workspaceLanguageValue` (if defined)
`workspaceFolderLanguageValue` (if defined)
```
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

## Hierarchy

* **WorkspaceConfiguration**

## Indexable

▪ [key: string]: any

Readable dictionary that backs this configuration.

- *Default Settings*
- *Global (User) Settings*
- *Workspace settings*
- *Workspace Folder settings* - From one of the [Workspace Folders](#workspace.workspaceFolders) under which requested resource belongs to.
- *Language settings* - Settings defined under requested language.

The *effective* value (returned by [`get`](#WorkspaceConfiguration.get)) is computed by overriding or merging the values in the following order.

```
`defaultValue`
`globalValue` (if defined)
`workspaceValue` (if defined)
`workspaceFolderValue` (if defined)
`defaultLanguageValue` (if defined)
`globalLanguageValue` (if defined)
`workspaceLanguageValue` (if defined)
`workspaceFolderLanguageValue` (if defined)
```
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

## Index

### Methods

* [get](_index_d_._plugin_.workspaceconfiguration.md#get)
* [has](_index_d_._plugin_.workspaceconfiguration.md#has)
* [inspect](_index_d_._plugin_.workspaceconfiguration.md#inspect)
* [update](_index_d_._plugin_.workspaceconfiguration.md#update)

## Methods

### get

▸ **get**\<T>(`section`: string): T \| undefined

*Defined in [index.d.ts:4697](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4697)*

Return a value from this configuration.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |

**Returns:** T \| undefined

The value `section` denotes or `undefined`.

▸ **get**\<T>(`section`: string, `defaultValue`: T): T

*Defined in [index.d.ts:4706](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4706)*

Return a value from this configuration.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |
`defaultValue` | T | A value should be returned when no value could be found, is `undefined`. |

**Returns:** T

The value `section` denotes or the default.

___

### has

▸ **has**(`section`: string): boolean

*Defined in [index.d.ts:4714](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4714)*

Check if this configuration has a certain value.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |

**Returns:** boolean

`true` if the section doesn't resolve to `undefined`.

___

### inspect

▸ **inspect**\<T>(`section`: string): { defaultLanguageValue?: T ; defaultValue?: T ; globalLanguageValue?: T ; globalValue?: T ; key: string ; languageIds?: string[] ; workspaceFolderLanguageValue?: T ; workspaceFolderValue?: T ; workspaceLanguageValue?: T ; workspaceValue?: T  } \| undefined

*Defined in [index.d.ts:4730](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4730)*

Retrieve all information about a configuration setting. A configuration value
often consists of a *default* value, a global or installation-wide value,
a workspace-specific value, folder-specific value
and language-specific values (if [WorkspaceConfiguration](#WorkspaceConfiguration) is scoped to a language).

Also provides all language ids under which the given configuration setting is defined.

*Note:* The configuration name must denote a leaf in the configuration tree
(`editor.fontSize` vs `editor`) otherwise no result is returned.

#### Type parameters:

Name |
------ |
`T` |

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |

**Returns:** { defaultLanguageValue?: T ; defaultValue?: T ; globalLanguageValue?: T ; globalValue?: T ; key: string ; languageIds?: string[] ; workspaceFolderLanguageValue?: T ; workspaceFolderValue?: T ; workspaceLanguageValue?: T ; workspaceValue?: T  } \| undefined

Information about a configuration setting or `undefined`.

___

### update

▸ **update**(`section`: string, `value`: any, `configurationTarget?`: [ConfigurationTarget](../enums/_index_d_._plugin_.configurationtarget.md) \| boolean, `overrideInLanguage?`: boolean): [Thenable](_index_d_.thenable.md)\<void>

*Defined in [index.d.ts:4776](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L4776)*

Update a configuration value. The updated configuration values are persisted.

A value can be changed in

- [Global settings](#ConfigurationTarget.Global): Changes the value for all instances of the editor.
- [Workspace settings](#ConfigurationTarget.Workspace): Changes the value for current workspace, if available.
- [Workspace folder settings](#ConfigurationTarget.WorkspaceFolder): Changes the value for settings from one of the [Workspace Folders](#workspace.workspaceFolders) under which the requested resource belongs to.
- Language settings: Changes the value for the requested languageId.

*Note:* To remove a configuration value use `undefined`, like so: `config.update('somekey', undefined)`

**`throws`** error while updating
	- configuration which is not registered.
	- window configuration to workspace folder
	- configuration to workspace or workspace folder when no workspace is opened.
	- configuration to workspace folder when there is no workspace folder settings.
	- configuration to workspace folder when [WorkspaceConfiguration](#WorkspaceConfiguration) is not scoped to a resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`section` | string | Configuration name, supports _dotted_ names. |
`value` | any | The new value. |
`configurationTarget?` | [ConfigurationTarget](../enums/_index_d_._plugin_.configurationtarget.md) \| boolean | The [configuration target](#ConfigurationTarget) or a boolean value.  - If `true` updates [Global settings](#ConfigurationTarget.Global).  - If `false` updates [Workspace settings](#ConfigurationTarget.Workspace).  - If `undefined` or `null` updates to [Workspace folder settings](#ConfigurationTarget.WorkspaceFolder) if configuration is resource specific,  otherwise to [Workspace settings](#ConfigurationTarget.Workspace). |
`overrideInLanguage?` | boolean | Whether to update the value in the scope of requested languageId or not.  - If `true` updates the value under the requested languageId.  - If `undefined` updates the value under the requested languageId only if the configuration is defined for the language. |

**Returns:** [Thenable](_index_d_.thenable.md)\<void>
