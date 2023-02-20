**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](../modules/_index_d_.md) / ["plugin"](../modules/_index_d_._plugin_.md) / WebviewOptions

# Interface: WebviewOptions

Content settings for a webview.

## Hierarchy

* **WebviewOptions**

## Index

### Properties

* [enableCommandUris](_index_d_._plugin_.webviewoptions.md#enablecommanduris)
* [enableScripts](_index_d_._plugin_.webviewoptions.md#enablescripts)
* [localResourceRoots](_index_d_._plugin_.webviewoptions.md#localresourceroots)
* [portMapping](_index_d_._plugin_.webviewoptions.md#portmapping)

## Properties

### enableCommandUris

• `Optional` `Readonly` **enableCommandUris**: boolean

*Defined in [index.d.ts:7239](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7239)*

Controls whether command uris are enabled in webview content or not.

Defaults to false.

___

### enableScripts

• `Optional` `Readonly` **enableScripts**: boolean

*Defined in [index.d.ts:7232](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7232)*

Controls whether scripts are enabled in the webview content or not.

Defaults to false (scripts-disabled).

___

### localResourceRoots

• `Optional` `Readonly` **localResourceRoots**: ReadonlyArray\<[Uri](../classes/_index_d_._plugin_.uri.md)>

*Defined in [index.d.ts:7248](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7248)*

Root paths from which the webview can load local (filesystem) resources using uris from `asWebviewUri`

Default to the root folders of the current workspace plus the extension's install directory.

Pass in an empty array to disallow access to any local resources.

___

### portMapping

• `Optional` `Readonly` **portMapping**: ReadonlyArray\<[WebviewPortMapping](_index_d_._plugin_.webviewportmapping.md)>

*Defined in [index.d.ts:7263](https://github.com/shuyaqian/cloudide-plugin-api/blob/6d83fa1/index.d.ts#L7263)*

Mappings of localhost ports used inside the webview.

Port mapping allow webviews to transparently define how localhost ports are resolved. This can be used
to allow using a static localhost port inside the webview that is resolved to random port that a service is
running on.

If a webview accesses localhost content, we recommend that you specify port mappings even if
the `webviewPort` and `extensionHostPort` ports are the same.

*Note* that port mappings only work for `http` or `https` urls. Websocket urls (e.g. `ws://localhost:3000`)
cannot be mapped to another port.
