[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CodeAction

# Class: CodeAction

["@codearts/plugin"](../modules/_codearts_plugin_.md).CodeAction

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CodeAction.md#constructor)

### Properties

- [command](codearts_plugin_.CodeAction.md#command)
- [diagnostics](codearts_plugin_.CodeAction.md#diagnostics)
- [disabled](codearts_plugin_.CodeAction.md#disabled)
- [edit](codearts_plugin_.CodeAction.md#edit)
- [isPreferred](codearts_plugin_.CodeAction.md#ispreferred)
- [kind](codearts_plugin_.CodeAction.md#kind)
- [title](codearts_plugin_.CodeAction.md#title)

## Constructors

### constructor

• **new CodeAction**(`title`, `kind?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `title` | `string` |  |
| `kind?` | [`CodeActionKind`](codearts_plugin_.CodeActionKind.md) |  |

#### Defined in

[index.d.ts:2477](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2477)

## Properties

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

#### Defined in

[index.d.ts:2428](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2428)

___

### diagnostics

• `Optional` **diagnostics**: [`Diagnostic`](codearts_plugin_.Diagnostic.md)[]

#### Defined in

[index.d.ts:2420](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2420)

___

### disabled

• `Optional` **disabled**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `reason` | `string` |  |

#### Defined in

[index.d.ts:2459](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2459)

___

### edit

• `Optional` **edit**: [`WorkspaceEdit`](codearts_plugin_.WorkspaceEdit.md)

#### Defined in

[index.d.ts:2415](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2415)

___

### isPreferred

• `Optional` **isPreferred**: `boolean`

#### Defined in

[index.d.ts:2444](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2444)

___

### kind

• `Optional` **kind**: [`CodeActionKind`](codearts_plugin_.CodeActionKind.md)

#### Defined in

[index.d.ts:2435](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2435)

___

### title

• **title**: `string`

#### Defined in

[index.d.ts:2410](https://github.com/huaweicloud/cloudide-plugin-api/blob/203b986/index.d.ts#L2410)
