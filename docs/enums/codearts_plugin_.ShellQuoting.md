[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ShellQuoting

# Enumeration: ShellQuoting

["@codearts/plugin"](../modules/_codearts_plugin_.md).ShellQuoting

Defines how an argument should be quoted if it contains
spaces or unsupported characters.

## Table of contents

### Enumeration Members

- [Escape](codearts_plugin_.ShellQuoting.md#escape)
- [Strong](codearts_plugin_.ShellQuoting.md#strong)
- [Weak](codearts_plugin_.ShellQuoting.md#weak)

## Enumeration Members

### Escape

• **Escape** = ``1``

Character escaping should be used. This for example
uses \ on bash and ` on PowerShell.

#### Defined in

[index.d.ts:7364](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7364)

___

### Strong

• **Strong** = ``2``

Strong string quoting should be used. This for example
uses " for Windows cmd and ' for bash and PowerShell.
Strong quoting treats arguments as literal strings.
Under PowerShell echo 'The value is $(2 * 3)' will
print `The value is $(2 * 3)`

#### Defined in

[index.d.ts:7373](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7373)

___

### Weak

• **Weak** = ``3``

Weak string quoting should be used. This for example
uses " for Windows cmd, bash and PowerShell. Weak quoting
still performs some kind of evaluation inside the quoted
string.  Under PowerShell echo "The value is $(2 * 3)"
will print `The value is 6`

#### Defined in

[index.d.ts:7382](https://github.com/huaweicloud/cloudide-plugin-api/blob/a055dd0/index.d.ts#L7382)
