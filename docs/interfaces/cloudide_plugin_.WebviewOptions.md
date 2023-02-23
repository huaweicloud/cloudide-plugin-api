[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](../modules/_cloudide_plugin_.md) / WebviewOptions

# Interface: WebviewOptions

["@cloudide/plugin"](../modules/_cloudide_plugin_.md).WebviewOptions

Content settings for a webview.

## Table of contents

### Properties

- [enableCommandUris](cloudide_plugin_.WebviewOptions.md#enablecommanduris)
- [enableScripts](cloudide_plugin_.WebviewOptions.md#enablescripts)
- [localResourceRoots](cloudide_plugin_.WebviewOptions.md#localresourceroots)
- [portMapping](cloudide_plugin_.WebviewOptions.md#portmapping)

## Properties

### enableCommandUris

• `Optional` `Readonly` **enableCommandUris**: `boolean`

Controls whether command uris are enabled in webview content or not.

Defaults to false.

#### Defined in

[index.d.ts:3387](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3387)

___

### enableScripts

• `Optional` `Readonly` **enableScripts**: `boolean`

Controls whether scripts are enabled in the webview content or not.

Defaults to false (scripts-disabled).

#### Defined in

[index.d.ts:3380](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3380)

___

### localResourceRoots

• `Optional` `Readonly` **localResourceRoots**: readonly [`Uri`](../classes/cloudide_plugin_.Uri.md)[]

Root paths from which the webview can load local (filesystem) resources using the `theia-resource:` scheme.

Default to the root folders of the current workspace plus the extension's install directory.

Pass in an empty array to disallow access to any local resources.

#### Defined in

[index.d.ts:3396](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3396)

___

### portMapping

• `Optional` `Readonly` **portMapping**: readonly [`WebviewPortMapping`](cloudide_plugin_.WebviewPortMapping.md)[]

Mappings of localhost ports used inside the webview.

Port mapping allow webviews to transparently define how localhost ports are resolved. This can be used
to allow using a static localhost port inside the webview that is resolved to random port that a service is
running on.

If a webview accesses localhost content, we recommend that you specify port mappings even if
the `webviewPort` and `extensionHostPort` ports are the same.

*Note* that port mappings only work for `http` or `https` urls. Websocket urls (e.g. `ws://localhost:3000`)
cannot be mapped to another port.

#### Defined in

[index.d.ts:3411](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L3411)
