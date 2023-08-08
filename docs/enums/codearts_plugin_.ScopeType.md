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

[index.d.ts:12198](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12198)

___

### LanguageOverridable

• **LanguageOverridable** = ``"language-overridable"``

Resource settings that can be overridable at a language level.

#### Defined in

[index.d.ts:12224](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12224)

___

### Machine

• **Machine** = ``"machine"``

Machine specific settings that can be set only in user settings or only in remote settings,
For example, an installation path which shouldn't be shared across machines.

#### Defined in

[index.d.ts:12204](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12204)

___

### MachineOverridable

• **MachineOverridable** = ``"machine-overridable"``

Machine specific settings that can be overridden by workspace or folder settings.

#### Defined in

[index.d.ts:12209](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12209)

___

### Resource

• **Resource** = ``"resource"``

Resource settings, which apply to files and folders, and can be configured in all settings levels, even folder settings.

#### Defined in

[index.d.ts:12219](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12219)

___

### Window

• **Window** = ``"window"``

Windows (instance) specific settings which can be configured in user, workspace, or remote settings.

#### Defined in

[index.d.ts:12214](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L12214)
