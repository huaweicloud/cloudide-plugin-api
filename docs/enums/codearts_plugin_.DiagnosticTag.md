[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / DiagnosticTag

# Enumeration: DiagnosticTag

["@codearts/plugin"](../modules/_codearts_plugin_.md).DiagnosticTag

Additional metadata about the type of a diagnostic.

## Table of contents

### Enumeration Members

- [Deprecated](codearts_plugin_.DiagnosticTag.md#deprecated)
- [Unnecessary](codearts_plugin_.DiagnosticTag.md#unnecessary)

## Enumeration Members

### Deprecated

• **Deprecated** = ``2``

Deprecated or obsolete code.

Diagnostics with this tag are rendered with a strike through.

#### Defined in

[index.d.ts:6010](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6010)

___

### Unnecessary

• **Unnecessary** = ``1``

Unused or unnecessary code.

Diagnostics with this tag are rendered faded out. The amount of fading
is controlled by the `"editorUnnecessaryCode.opacity"` theme color. For
example, `"editorUnnecessaryCode.opacity": "#000000c0"` will render the
code with 75% opacity. For high contrast themes, use the
`"editorUnnecessaryCode.border"` theme color to underline unnecessary code
instead of fading it out.

#### Defined in

[index.d.ts:6003](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L6003)
