**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / ExtensionMode

# Enumeration: ExtensionMode

The ExtensionMode is provided on the `ExtensionContext` and indicates the
mode the specific extension is running in.

## Index

### Enumeration members

* [Development](_index_d_._plugin_.extensionmode.md#development)
* [Production](_index_d_._plugin_.extensionmode.md#production)
* [Test](_index_d_._plugin_.extensionmode.md#test)

## Enumeration members

### Development

•  **Development**:  = 2

*Defined in [index.d.ts:5898](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5898)*

The extension is running from an `--extensionDevelopmentPath` provided
when launching VS Code.

___

### Production

•  **Production**:  = 1

*Defined in [index.d.ts:5892](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5892)*

The extension is installed normally (for example, from the marketplace
or VSIX) in VS Code.

___

### Test

•  **Test**:  = 3

*Defined in [index.d.ts:5904](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L5904)*

The extension is running from an `--extensionTestsPath` and
the extension host is running unit tests.
