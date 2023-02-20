**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / DiagnosticTag

# Enumeration: DiagnosticTag

Additional metadata about the type of a diagnostic.

## Index

### Enumeration members

* [Deprecated](_index_d_._plugin_.diagnostictag.md#deprecated)
* [Unnecessary](_index_d_._plugin_.diagnostictag.md#unnecessary)

## Enumeration members

### Deprecated

•  **Deprecated**:  = 2

*Defined in [index.d.ts:5220](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5220)*

Deprecated or obsolete code.

Diagnostics with this tag are rendered with a strike through.

___

### Unnecessary

•  **Unnecessary**:  = 1

*Defined in [index.d.ts:5213](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5213)*

Unused or unnecessary code.

Diagnostics with this tag are rendered faded out. The amount of fading
is controlled by the `"editorUnnecessaryCode.opacity"` theme color. For
example, `"editorUnnecessaryCode.opacity": "#000000c0"` will render the
code with 75% opacity. For high contrast themes, use the
`"editorUnnecessaryCode.border"` theme color to underline unnecessary code
instead of fading it out.
