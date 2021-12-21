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

*Defined in [index.d.ts:6357](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6357)*

The character used to do character escaping. If a string is provided only spaces
are escaped. If a `{ escapeChar, charsToEscape }` literal is provide all characters
in `charsToEscape` are escaped using the `escapeChar`.

___

### strong

• `Optional` **strong**: string

*Defined in [index.d.ts:6371](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6371)*

The character used for strong quoting. The string's length must be 1.

___

### weak

• `Optional` **weak**: string

*Defined in [index.d.ts:6376](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6376)*

The character used for weak quoting. The string's length must be 1.
