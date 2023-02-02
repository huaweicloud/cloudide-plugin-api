[@codearts/plugin](../README.md) / ["@codearts/plugin"](../modules/_codearts_plugin_.md) / WebviewOptions

# Interface: WebviewOptions

["@codearts/plugin"](../modules/_codearts_plugin_.md).WebviewOptions

Content settings for a webview.

## Table of contents

### Properties

- [enableCommandUris](codearts_plugin_.WebviewOptions.md#enablecommanduris)
- [enableForms](codearts_plugin_.WebviewOptions.md#enableforms)
- [enableScripts](codearts_plugin_.WebviewOptions.md#enablescripts)
- [localResourceRoots](codearts_plugin_.WebviewOptions.md#localresourceroots)
- [portMapping](codearts_plugin_.WebviewOptions.md#portmapping)

## Properties

### enableCommandUris

• `Optional` `Readonly` **enableCommandUris**: `boolean`

Controls whether command uris are enabled in webview content or not.

Defaults to false.

#### Defined in

[index.d.ts:8270](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8270)

___

### enableForms

• `Optional` `Readonly` **enableForms**: `boolean`

Controls whether forms are enabled in the webview content or not.

Defaults to true if [scripts are enabled](codearts_plugin_.WebviewOptions.md#enablescripts). Otherwise defaults to false.
Explicitly setting this property to either true or false overrides the default.

#### Defined in

[index.d.ts:8263](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8263)

___

### enableScripts

• `Optional` `Readonly` **enableScripts**: `boolean`

Controls whether scripts are enabled in the webview content or not.

Defaults to false (scripts-disabled).

#### Defined in

[index.d.ts:8255](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8255)

___

### localResourceRoots

• `Optional` `Readonly` **localResourceRoots**: readonly [`Uri`](../classes/codearts_plugin_.Uri.md)[]

Root paths from which the webview can load local (filesystem) resources using uris from `asWebviewUri`

Default to the root folders of the current workspace plus the extension's install directory.

Pass in an empty array to disallow access to any local resources.

#### Defined in

[index.d.ts:8279](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8279)

___

### portMapping

• `Optional` `Readonly` **portMapping**: readonly [`WebviewPortMapping`](codearts_plugin_.WebviewPortMapping.md)[]

Mappings of localhost ports used inside the webview.

Port mapping allow webviews to transparently define how localhost ports are resolved. This can be used
to allow using a static localhost port inside the webview that is resolved to random port that a service is
running on.

If a webview accesses localhost content, we recommend that you specify port mappings even if
the `webviewPort` and `extensionHostPort` ports are the same.

*Note* that port mappings only work for `http` or `https` urls. Websocket urls (e.g. `ws://localhost:3000`)
cannot be mapped to another port.

#### Defined in

[index.d.ts:8294](https://github.com/huaweicloud/cloudide-plugin-api/blob/03b481c/index.d.ts#L8294)
