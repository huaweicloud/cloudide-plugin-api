**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ShellQuoting

# Enumeration: ShellQuoting

Defines how an argument should be quoted if it contains
spaces or unsupported characters.

## Index

### Enumeration members

* [Escape](_index_d_._plugin_.shellquoting.md#escape)
* [Strong](_index_d_._plugin_.shellquoting.md#strong)
* [Weak](_index_d_._plugin_.shellquoting.md#weak)

## Enumeration members

### Escape

•  **Escape**:  = 1

*Defined in [index.d.ts:6425](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6425)*

Character escaping should be used. This for example
uses \ on bash and ` on PowerShell.

___

### Strong

•  **Strong**:  = 2

*Defined in [index.d.ts:6434](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6434)*

Strong string quoting should be used. This for example
uses " for Windows cmd and ' for bash and PowerShell.
Strong quoting treats arguments as literal strings.
Under PowerShell echo 'The value is $(2 * 3)' will
print `The value is $(2 * 3)`

___

### Weak

•  **Weak**:  = 3

*Defined in [index.d.ts:6443](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6443)*

Weak string quoting should be used. This for example
uses " for Windows cmd, bash and PowerShell. Weak quoting
still performs some kind of evaluation inside the quoted
string.  Under PowerShell echo "The value is $(2 * 3)"
will print `The value is 6`
