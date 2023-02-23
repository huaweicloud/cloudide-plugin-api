[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / ExtensionMode

# Enumeration: ExtensionMode

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).ExtensionMode

The ExtensionMode is provided on the `ExtensionContext` and indicates the
mode the specific extension is running in.

## Table of contents

### Enumeration Members

- [Development](cloudide_plugin_.ExtensionMode.md#development)
- [Production](cloudide_plugin_.ExtensionMode.md#production)
- [Test](cloudide_plugin_.ExtensionMode.md#test)

## Enumeration Members

### Development

• **Development** = ``2``

The extension is running from an `--extensionDevelopmentPath` provided
when launching the editor.

#### Defined in

[index.d.ts:3137](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3137)

___

### Production

• **Production** = ``1``

The extension is installed normally (for example, from the marketplace
or VSIX) in the editor.

#### Defined in

[index.d.ts:3131](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3131)

___

### Test

• **Test** = ``3``

The extension is running from an `--extensionTestsPath` and
the extension host is running unit tests.

#### Defined in

[index.d.ts:3143](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3143)
