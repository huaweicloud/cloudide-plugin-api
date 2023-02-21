[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / LanguageConfiguration

# Interface: LanguageConfiguration

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).LanguageConfiguration

The language configuration interfaces defines the contract between extensions
and various editor features, like automatic bracket insertion, automatic indentation etc.

## Table of contents

### Properties

- [\_\_characterPairSupport](cloudide_plugin_.LanguageConfiguration.md#__characterpairsupport)
- [\_\_electricCharacterSupport](cloudide_plugin_.LanguageConfiguration.md#__electriccharactersupport)
- [brackets](cloudide_plugin_.LanguageConfiguration.md#brackets)
- [comments](cloudide_plugin_.LanguageConfiguration.md#comments)
- [indentationRules](cloudide_plugin_.LanguageConfiguration.md#indentationrules)
- [onEnterRules](cloudide_plugin_.LanguageConfiguration.md#onenterrules)
- [wordPattern](cloudide_plugin_.LanguageConfiguration.md#wordpattern)

## Properties

### \_\_characterPairSupport

• `Optional` **\_\_characterPairSupport**: `Object`

**`Deprecated`**

Use the autoClosingPairs property in the language configuration file instead.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `autoClosingPairs` | { `close`: `String` ; `notIn`: `String`[] ; `open`: `String`  }[] |

#### Defined in

[index.d.ts:6691](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6691)

___

### \_\_electricCharacterSupport

• `Optional` **\_\_electricCharacterSupport**: `Object`

**`Deprecated`**

Do not use. Will be replaced by a better API soon.

#### Type declaration

| Name | Type |
| :------ | :------ |
| `brackets` | `any` |
| `docComment` | { `close`: `String` ; `lineStart`: `String` ; `open`: `String` ; `scope`: `String`  } |
| `docComment.close` | `String` |
| `docComment.lineStart` | `String` |
| `docComment.open` | `String` |
| `docComment.scope` | `String` |

#### Defined in

[index.d.ts:6695](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6695)

___

### brackets

• `Optional` **brackets**: [`CharacterPair`](../modules/_cloudide_plugin_.md#characterpair)[]

The language's brackets.
This configuration implicitly affects pressing Enter around these brackets.

#### Defined in

[index.d.ts:6704](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6704)

___

### comments

• `Optional` **comments**: [`CommentRule`](cloudide_plugin_.CommentRule.md)

The language's comment settings.

#### Defined in

[index.d.ts:6699](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6699)

___

### indentationRules

• `Optional` **indentationRules**: [`IndentationRule`](cloudide_plugin_.IndentationRule.md)

The language's indentation settings.

#### Defined in

[index.d.ts:6716](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6716)

___

### onEnterRules

• `Optional` **onEnterRules**: [`OnEnterRule`](cloudide_plugin_.OnEnterRule.md)[]

The language's rules to be evaluated when pressing Enter.

#### Defined in

[index.d.ts:6720](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6720)

___

### wordPattern

• `Optional` **wordPattern**: `RegExp`

The language's word definition.
If the language supports Unicode identifiers (e.g. JavaScript), it is preferable
to provide a word definition that uses exclusion of known separators.
e.g.: A regex that matches anything except known separators (and dot is allowed to occur in a floating point number):
  /(-?\d*\.\d\w*)|([^`\~\!@\#\%\^\&\*\(\)\-\=\+\[{\]}\\\|\;\:\'\"\,\.\<\>/\?\s]+)/g

#### Defined in

[index.d.ts:6712](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L6712)
