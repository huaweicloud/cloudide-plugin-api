[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LanguageConfiguration

# Interface: LanguageConfiguration

["@codearts/plugin"](../modules/_codearts_plugin_.md).LanguageConfiguration

## Table of contents

### Properties

- [\_\_characterPairSupport](codearts_plugin_.LanguageConfiguration.md#__characterpairsupport)
- [\_\_electricCharacterSupport](codearts_plugin_.LanguageConfiguration.md#__electriccharactersupport)
- [brackets](codearts_plugin_.LanguageConfiguration.md#brackets)
- [comments](codearts_plugin_.LanguageConfiguration.md#comments)
- [indentationRules](codearts_plugin_.LanguageConfiguration.md#indentationrules)
- [onEnterRules](codearts_plugin_.LanguageConfiguration.md#onenterrules)
- [wordPattern](codearts_plugin_.LanguageConfiguration.md#wordpattern)

## Properties

### \_\_characterPairSupport

• `Optional` **\_\_characterPairSupport**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `autoClosingPairs` | { `close`: `string` ; `notIn?`: `string`[] ; `open`: `string`  }[] |

#### Defined in

[index.d.ts:5589](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5589)

___

### \_\_electricCharacterSupport

• `Optional` **\_\_electricCharacterSupport**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `brackets?` | `any` |  |
| `docComment?` | { `close?`: `string` ; `lineStart`: `string` ; `open`: `string` ; `scope`: `string`  } |  |
| `docComment.close?` | `string` | - |
| `docComment.lineStart` | `string` | - |
| `docComment.open` | `string` | - |
| `docComment.scope` | `string` | - |

#### Defined in

[index.d.ts:5563](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5563)

___

### brackets

• `Optional` **brackets**: [`CharacterPair`](../modules/_codearts_plugin_.md#characterpair)[]

#### Defined in

[index.d.ts:5540](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5540)

___

### comments

• `Optional` **comments**: [`CommentRule`](codearts_plugin_.CommentRule.md)

#### Defined in

[index.d.ts:5535](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5535)

___

### indentationRules

• `Optional` **indentationRules**: [`IndentationRule`](codearts_plugin_.IndentationRule.md)

#### Defined in

[index.d.ts:5552](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5552)

___

### onEnterRules

• `Optional` **onEnterRules**: [`OnEnterRule`](codearts_plugin_.OnEnterRule.md)[]

#### Defined in

[index.d.ts:5556](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5556)

___

### wordPattern

• `Optional` **wordPattern**: `RegExp`

#### Defined in

[index.d.ts:5548](https://github.com/huaweicloud/cloudide-plugin-api/blob/84e382d/index.d.ts#L5548)
