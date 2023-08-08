[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / ExtensionMode

# Enumeration: ExtensionMode

["@codearts/plugin"](../modules/_codearts_plugin_.md).ExtensionMode

The ExtensionMode is provided on the `ExtensionContext` and indicates the
mode the specific extension is running in.

## Table of contents

### Enumeration Members

- [Development](codearts_plugin_.ExtensionMode.md#development)
- [Production](codearts_plugin_.ExtensionMode.md#production)
- [Test](codearts_plugin_.ExtensionMode.md#test)

## Enumeration Members

### Development

• **Development** = ``2``

The extension is running from an `--extensionDevelopmentPath` provided
when launching the editor.

#### Defined in

[index.d.ts:6902](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6902)

___

### Production

• **Production** = ``1``

The extension is installed normally (for example, from the marketplace
or VSIX) in the editor.

#### Defined in

[index.d.ts:6896](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6896)

___

### Test

• **Test** = ``3``

The extension is running from an `--extensionTestsPath` and
the extension host is running unit tests.

#### Defined in

[index.d.ts:6908](https://github.com/xyz-fish/cloudide-plugin-api/blob/9927cd6/index.d.ts#L6908)
