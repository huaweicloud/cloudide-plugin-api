[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ShellExecution

# Class: ShellExecution

["@codearts/plugin"](../modules/_codearts_plugin_.md).ShellExecution

## Table of contents

### Constructors

- [constructor](codearts_plugin_.ShellExecution.md#constructor)

### Properties

- [args](codearts_plugin_.ShellExecution.md#args)
- [command](codearts_plugin_.ShellExecution.md#command)
- [commandLine](codearts_plugin_.ShellExecution.md#commandline)
- [options](codearts_plugin_.ShellExecution.md#options)

## Constructors

### constructor

• **new ShellExecution**(`commandLine`, `options?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `commandLine` | `string` |  |
| `options?` | [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md) |  |

#### Defined in

[index.d.ts:7407](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7407)

• **new ShellExecution**(`command`, `args`, `options?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `command` | `string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md) |  |
| `args` | (`string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md))[] |  |
| `options?` | [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md) |  |

#### Defined in

[index.d.ts:7419](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7419)

## Properties

### args

• **args**: (`string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md))[]

#### Defined in

[index.d.ts:7434](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7434)

___

### command

• **command**: `string` \| [`ShellQuotedString`](../interfaces/codearts_plugin_.ShellQuotedString.md)

#### Defined in

[index.d.ts:7429](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7429)

___

### commandLine

• **commandLine**: `undefined` \| `string`

#### Defined in

[index.d.ts:7424](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7424)

___

### options

• `Optional` **options**: [`ShellExecutionOptions`](../interfaces/codearts_plugin_.ShellExecutionOptions.md)

#### Defined in

[index.d.ts:7440](https://github.com/huaweicloud/cloudide-plugin-api/blob/03c74e5/index.d.ts#L7440)
