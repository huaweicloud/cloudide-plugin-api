[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ShellQuotingOptions

# Interface: ShellQuotingOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).ShellQuotingOptions

The shell quoting options.

## Table of contents

### Properties

- [escape](codearts_plugin_.ShellQuotingOptions.md#escape)
- [strong](codearts_plugin_.ShellQuotingOptions.md#strong)
- [weak](codearts_plugin_.ShellQuotingOptions.md#weak)

## Properties

### escape

• `Optional` **escape**: `string` \| { `charsToEscape`: `string` ; `escapeChar`: `string`  }

The character used to do character escaping. If a string is provided only spaces
are escaped. If a `{ escapeChar, charsToEscape }` literal is provide all characters
in `charsToEscape` are escaped using the `escapeChar`.

#### Defined in

[index.d.ts:7321](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7321)

___

### strong

• `Optional` **strong**: `string`

The character used for strong quoting. The string's length must be 1.

#### Defined in

[index.d.ts:7335](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7335)

___

### weak

• `Optional` **weak**: `string`

The character used for weak quoting. The string's length must be 1.

#### Defined in

[index.d.ts:7340](https://github.com/huaweicloud/cloudide-plugin-api/blob/4d28848/index.d.ts#L7340)
