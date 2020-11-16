**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ShellQuotingOptions

# Interface: ShellQuotingOptions

The shell quoting options.

## Hierarchy

* **ShellQuotingOptions**

## Index

### Properties

* [escape](_index_d_._plugin_.shellquotingoptions.md#escape)
* [strong](_index_d_._plugin_.shellquotingoptions.md#strong)
* [weak](_index_d_._plugin_.shellquotingoptions.md#weak)

## Properties

### escape

• `Optional` **escape**: string \| { charsToEscape: string ; escapeChar: string  }

*Defined in [index.d.ts:5759](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5759)*

The character used to do character escaping. If a string is provided only spaces
are escaped. If a `{ escapeChar, charsToEscape }` literal is provide all characters
in `charsToEscape` are escaped using the `escapeChar`.

___

### strong

• `Optional` **strong**: string

*Defined in [index.d.ts:5773](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5773)*

The character used for strong quoting. The string's length must be 1.

___

### weak

• `Optional` **weak**: string

*Defined in [index.d.ts:5778](https://github.com/huaweicloud/cloudide-plugin-api/blob/1ab5ef8/index.d.ts#L5778)*

The character used for weak quoting. The string's length must be 1.
