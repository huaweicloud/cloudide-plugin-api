[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ShellQuotingOptions

# Interface: ShellQuotingOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ShellQuotingOptions

## Table of contents

### Properties

- [escape](cloudide_plugin_.ShellQuotingOptions.md#escape)
- [strong](cloudide_plugin_.ShellQuotingOptions.md#strong)
- [weak](cloudide_plugin_.ShellQuotingOptions.md#weak)

## Properties

### escape

• `Optional` **escape**: `string` \| { `charsToEscape`: `string` ; `escapeChar`: `string`  }

The character used to do character escaping. If a string is provided only spaces
are escaped. If a `{ escapeChar, charsToEscape }` literal is provide all characters
in `charsToEscape` are escaped using the `escapeChar`.

#### Defined in

[index.d.ts:10224](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10224)

___

### strong

• `Optional` **strong**: `string`

The character used for strong quoting. The string's length must be 1

#### Defined in

[index.d.ts:10233](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10233)

___

### weak

• `Optional` **weak**: `string`

The character used for weak quoting. The string's length must be 1

#### Defined in

[index.d.ts:10236](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10236)
