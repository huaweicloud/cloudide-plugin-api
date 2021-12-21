**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / TaskRevealKind

# Enumeration: TaskRevealKind

Controls the behaviour of the terminal's visibility.

## Index

### Enumeration members

* [Always](_index_d_._plugin_.taskrevealkind.md#always)
* [Never](_index_d_._plugin_.taskrevealkind.md#never)
* [Silent](_index_d_._plugin_.taskrevealkind.md#silent)

## Enumeration members

### Always

•  **Always**:  = 1

*Defined in [index.d.ts:6157](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6157)*

Always brings the terminal to front if the task is executed.

___

### Never

•  **Never**:  = 3

*Defined in [index.d.ts:6168](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6168)*

The terminal never comes to front when the task is executed.

___

### Silent

•  **Silent**:  = 2

*Defined in [index.d.ts:6163](https://github.com/shuyaqian/cloudide-plugin-api/blob/57a3a2a/index.d.ts#L6163)*

Only brings the terminal to front if a problem is detected executing the task
(e.g. the task couldn't be started because).
