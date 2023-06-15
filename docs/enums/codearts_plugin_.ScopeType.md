[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ScopeType

# Enumeration: ScopeType

["@codearts/plugin"](../modules/_codearts_plugin_.md).ScopeType

## Table of contents

### Enumeration Members

- [Application](codearts_plugin_.ScopeType.md#application)
- [LanguageOverridable](codearts_plugin_.ScopeType.md#languageoverridable)
- [Machine](codearts_plugin_.ScopeType.md#machine)
- [MachineOverridable](codearts_plugin_.ScopeType.md#machineoverridable)
- [Resource](codearts_plugin_.ScopeType.md#resource)
- [Window](codearts_plugin_.ScopeType.md#window)

## Enumeration Members

### Application

• **Application** = ``"application"``

Settings that apply to all instances of CodeArts and can only be configured in user settings.

#### Defined in

[index.d.ts:12096](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12096)

___

### LanguageOverridable

• **LanguageOverridable** = ``"language-overridable"``

Resource settings that can be overridable at a language level.

#### Defined in

[index.d.ts:12122](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12122)

___

### Machine

• **Machine** = ``"machine"``

Machine specific settings that can be set only in user settings or only in remote settings,
For example, an installation path which shouldn't be shared across machines.

#### Defined in

[index.d.ts:12102](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12102)

___

### MachineOverridable

• **MachineOverridable** = ``"machine-overridable"``

Machine specific settings that can be overridden by workspace or folder settings.

#### Defined in

[index.d.ts:12107](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12107)

___

### Resource

• **Resource** = ``"resource"``

Resource settings, which apply to files and folders, and can be configured in all settings levels, even folder settings.

#### Defined in

[index.d.ts:12117](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12117)

___

### Window

• **Window** = ``"window"``

Windows (instance) specific settings which can be configured in user, workspace, or remote settings.

#### Defined in

[index.d.ts:12112](https://github.com/shuyaqian/cloudide-plugin-api/blob/5b69219/index.d.ts#L12112)
