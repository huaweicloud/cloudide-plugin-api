[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / LanguageConfiguration

# Interface: LanguageConfiguration

["@codearts/plugin"](../modules/_codearts_plugin_.md).LanguageConfiguration

The language configuration interfaces defines the contract between extensions
and various editor features, like automatic bracket insertion, automatic indentation etc.

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

**Deprecated** Do not use.

**`Deprecated`**

* Use the autoClosingPairs property in the language configuration file instead.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `autoClosingPairs` | { `close`: `string` ; `notIn?`: `string`[] ; `open`: `string`  }[] |

#### Defined in

[index.d.ts:5609](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5609)

___

### \_\_electricCharacterSupport

• `Optional` **\_\_electricCharacterSupport**: `Object`

**Deprecated** Do not use.

**`Deprecated`**

Will be replaced by a better API soon.

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `brackets?` | `any` | This property is deprecated and will be **ignored** from the editor.  **`Deprecated`** |
| `docComment?` | { `close?`: `string` ; `lineStart`: `string` ; `open`: `string` ; `scope`: `string`  } | This property is deprecated and not fully supported anymore by the editor (scope and lineStart are ignored). Use the autoClosingPairs property in the language configuration file instead.  **`Deprecated`** |
| `docComment.close?` | `string` | - |
| `docComment.lineStart` | `string` | - |
| `docComment.open` | `string` | - |
| `docComment.scope` | `string` | - |

#### Defined in

[index.d.ts:5583](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5583)

___

### brackets

• `Optional` **brackets**: [`CharacterPair`](../modules/_codearts_plugin_.md#characterpair)[]

The language's brackets.
This configuration implicitly affects pressing Enter around these brackets.

#### Defined in

[index.d.ts:5560](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5560)

___

### comments

• `Optional` **comments**: [`CommentRule`](codearts_plugin_.CommentRule.md)

The language's comment settings.

#### Defined in

[index.d.ts:5555](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5555)

___

### indentationRules

• `Optional` **indentationRules**: [`IndentationRule`](codearts_plugin_.IndentationRule.md)

The language's indentation settings.

#### Defined in

[index.d.ts:5572](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5572)

___

### onEnterRules

• `Optional` **onEnterRules**: [`OnEnterRule`](codearts_plugin_.OnEnterRule.md)[]

The language's rules to be evaluated when pressing Enter.

#### Defined in

[index.d.ts:5576](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5576)

___

### wordPattern

• `Optional` **wordPattern**: `RegExp`

The language's word definition.
If the language supports Unicode identifiers (e.g. JavaScript), it is preferable
to provide a word definition that uses exclusion of known separators.
e.g.: A regex that matches anything except known separators (and dot is allowed to occur in a floating point number):
  /(-?\d*\.\d\w*)|([^`\~\!@\#\%\^\&\*\(\)\-\=\+\[{\]}\\\|\;\:\'\"\,\.\<\>/\?\s]+)/g

#### Defined in

[index.d.ts:5568](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L5568)
