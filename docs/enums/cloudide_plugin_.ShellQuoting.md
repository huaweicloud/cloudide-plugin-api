[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ShellQuoting

# Enumeration: ShellQuoting

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ShellQuoting

## Table of contents

### Enumeration Members

- [Escape](cloudide_plugin_.ShellQuoting.md#escape)
- [Strong](cloudide_plugin_.ShellQuoting.md#strong)
- [Weak](cloudide_plugin_.ShellQuoting.md#weak)

## Enumeration Members

### Escape

• **Escape** = ``1``

Character escaping should be used. This for example
uses \ on bash and ` on PowerShell.

#### Defined in

[index.d.ts:10187](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10187)

___

### Strong

• **Strong** = ``2``

Strong string quoting should be used. This for example
uses " for Windows cmd and ' for bash and PowerShell.
Strong quoting treats arguments as literal strings.
Under PowerShell echo 'The value is $(2 * 3)' will
print `The value is $(2 * 3)`

#### Defined in

[index.d.ts:10196](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10196)

___

### Weak

• **Weak** = ``3``

Weak string quoting should be used. This for example
uses " for Windows cmd, bash and PowerShell. Weak quoting
still performs some kind of evaluation inside the quoted
string.  Under PowerShell echo "The value is $(2 * 3)"
will print `The value is 6`

#### Defined in

[index.d.ts:10205](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L10205)
