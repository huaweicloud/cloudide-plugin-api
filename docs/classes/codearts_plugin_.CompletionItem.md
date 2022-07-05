[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / CompletionItem

# Class: CompletionItem

["@codearts/plugin"](../modules/_codearts_plugin_.md).CompletionItem

## Table of contents

### Constructors

- [constructor](codearts_plugin_.CompletionItem.md#constructor)

### Properties

- [additionalTextEdits](codearts_plugin_.CompletionItem.md#additionaltextedits)
- [command](codearts_plugin_.CompletionItem.md#command)
- [commitCharacters](codearts_plugin_.CompletionItem.md#commitcharacters)
- [detail](codearts_plugin_.CompletionItem.md#detail)
- [documentation](codearts_plugin_.CompletionItem.md#documentation)
- [filterText](codearts_plugin_.CompletionItem.md#filtertext)
- [insertText](codearts_plugin_.CompletionItem.md#inserttext)
- [keepWhitespace](codearts_plugin_.CompletionItem.md#keepwhitespace)
- [kind](codearts_plugin_.CompletionItem.md#kind)
- [label](codearts_plugin_.CompletionItem.md#label)
- [preselect](codearts_plugin_.CompletionItem.md#preselect)
- [range](codearts_plugin_.CompletionItem.md#range)
- [sortText](codearts_plugin_.CompletionItem.md#sorttext)
- [tags](codearts_plugin_.CompletionItem.md#tags)
- [textEdit](codearts_plugin_.CompletionItem.md#textedit)

## Constructors

### constructor

• **new CompletionItem**(`label`, `kind?`)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `label` | `string` \| [`CompletionItemLabel`](../interfaces/codearts_plugin_.CompletionItemLabel.md) |  |
| `kind?` | [`CompletionItemKind`](../enums/codearts_plugin_.CompletionItemKind.md) |  |

#### Defined in

[index.d.ts:4393](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4393)

## Properties

### additionalTextEdits

• `Optional` **additionalTextEdits**: [`TextEdit`](codearts_plugin_.TextEdit.md)[]

#### Defined in

[index.d.ts:4375](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4375)

___

### command

• `Optional` **command**: [`Command`](../interfaces/codearts_plugin_.Command.md)

#### Defined in

[index.d.ts:4382](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4382)

___

### commitCharacters

• `Optional` **commitCharacters**: `string`[]

#### Defined in

[index.d.ts:4349](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4349)

___

### detail

• `Optional` **detail**: `string`

#### Defined in

[index.d.ts:4286](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4286)

___

### documentation

• `Optional` **documentation**: `string` \| [`MarkdownString`](codearts_plugin_.MarkdownString.md)

#### Defined in

[index.d.ts:4291](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4291)

___

### filterText

• `Optional` **filterText**: `string`

#### Defined in

[index.d.ts:4315](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4315)

___

### insertText

• `Optional` **insertText**: `string` \| [`SnippetString`](codearts_plugin_.SnippetString.md)

#### Defined in

[index.d.ts:4329](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4329)

___

### keepWhitespace

• `Optional` **keepWhitespace**: `boolean`

#### Defined in

[index.d.ts:4356](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4356)

___

### kind

• `Optional` **kind**: [`CompletionItemKind`](../enums/codearts_plugin_.CompletionItemKind.md)

#### Defined in

[index.d.ts:4275](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4275)

___

### label

• **label**: `string` \| [`CompletionItemLabel`](../interfaces/codearts_plugin_.CompletionItemLabel.md)

#### Defined in

[index.d.ts:4269](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4269)

___

### preselect

• `Optional` **preselect**: `boolean`

#### Defined in

[index.d.ts:4322](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4322)

___

### range

• `Optional` **range**: [`Range`](codearts_plugin_.Range.md) \| { `inserting`: [`Range`](codearts_plugin_.Range.md) ; `replacing`: [`Range`](codearts_plugin_.Range.md)  }

#### Defined in

[index.d.ts:4342](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4342)

___

### sortText

• `Optional` **sortText**: `string`

#### Defined in

[index.d.ts:4305](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4305)

___

### tags

• `Optional` **tags**: readonly [`Deprecated`](../enums/codearts_plugin_.CompletionItemTag.md#deprecated)[]

#### Defined in

[index.d.ts:4280](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4280)

___

### textEdit

• `Optional` **textEdit**: [`TextEdit`](codearts_plugin_.TextEdit.md)

#### Defined in

[index.d.ts:4368](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L4368)
