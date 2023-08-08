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

[index.d.ts:5647](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5647)

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

[index.d.ts:5621](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5621)

___

### brackets

• `Optional` **brackets**: [`CharacterPair`](../modules/_codearts_plugin_.md#characterpair)[]

The language's brackets.
This configuration implicitly affects pressing Enter around these brackets.

#### Defined in

[index.d.ts:5598](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5598)

___

### comments

• `Optional` **comments**: [`CommentRule`](codearts_plugin_.CommentRule.md)

The language's comment settings.

#### Defined in

[index.d.ts:5593](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5593)

___

### indentationRules

• `Optional` **indentationRules**: [`IndentationRule`](codearts_plugin_.IndentationRule.md)

The language's indentation settings.

#### Defined in

[index.d.ts:5610](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5610)

___

### onEnterRules

• `Optional` **onEnterRules**: [`OnEnterRule`](codearts_plugin_.OnEnterRule.md)[]

The language's rules to be evaluated when pressing Enter.

#### Defined in

[index.d.ts:5614](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5614)

___

### wordPattern

• `Optional` **wordPattern**: `RegExp`

The language's word definition.
If the language supports Unicode identifiers (e.g. JavaScript), it is preferable
to provide a word definition that uses exclusion of known separators.
e.g.: A regex that matches anything except known separators (and dot is allowed to occur in a floating point number):
  /(-?\d*\.\d\w*)|([^`\~\!@\#\%\^\&\*\(\)\-\=\+\[{\]}\\\|\;\:\'\"\,\.\<\>/\?\s]+)/g

#### Defined in

[index.d.ts:5606](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L5606)
