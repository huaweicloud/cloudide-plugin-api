[@cloudide/plugin](../README.md) / ["@cloudide/plugin"](_cloudide_plugin_.md) / languages

# Namespace: languages

["@cloudide/plugin"](_cloudide_plugin_.md).languages

## Table of contents

### Functions

- [createDiagnosticCollection](cloudide_plugin_.languages.md#creatediagnosticcollection)
- [getDiagnostics](cloudide_plugin_.languages.md#getdiagnostics)
- [getLanguages](cloudide_plugin_.languages.md#getlanguages)
- [match](cloudide_plugin_.languages.md#match)
- [onDidChangeDiagnostics](cloudide_plugin_.languages.md#ondidchangediagnostics)
- [registerCallHierarchyProvider](cloudide_plugin_.languages.md#registercallhierarchyprovider)
- [registerCodeActionsProvider](cloudide_plugin_.languages.md#registercodeactionsprovider)
- [registerCodeLensProvider](cloudide_plugin_.languages.md#registercodelensprovider)
- [registerColorProvider](cloudide_plugin_.languages.md#registercolorprovider)
- [registerCompletionItemProvider](cloudide_plugin_.languages.md#registercompletionitemprovider)
- [registerDeclarationProvider](cloudide_plugin_.languages.md#registerdeclarationprovider)
- [registerDefinitionProvider](cloudide_plugin_.languages.md#registerdefinitionprovider)
- [registerDocumentFormattingEditProvider](cloudide_plugin_.languages.md#registerdocumentformattingeditprovider)
- [registerDocumentHighlightProvider](cloudide_plugin_.languages.md#registerdocumenthighlightprovider)
- [registerDocumentLinkProvider](cloudide_plugin_.languages.md#registerdocumentlinkprovider)
- [registerDocumentRangeFormattingEditProvider](cloudide_plugin_.languages.md#registerdocumentrangeformattingeditprovider)
- [registerDocumentRangeSemanticTokensProvider](cloudide_plugin_.languages.md#registerdocumentrangesemantictokensprovider)
- [registerDocumentSemanticTokensProvider](cloudide_plugin_.languages.md#registerdocumentsemantictokensprovider)
- [registerDocumentSymbolProvider](cloudide_plugin_.languages.md#registerdocumentsymbolprovider)
- [registerFoldingRangeProvider](cloudide_plugin_.languages.md#registerfoldingrangeprovider)
- [registerHoverProvider](cloudide_plugin_.languages.md#registerhoverprovider)
- [registerImplementationProvider](cloudide_plugin_.languages.md#registerimplementationprovider)
- [registerOnTypeFormattingEditProvider](cloudide_plugin_.languages.md#registerontypeformattingeditprovider)
- [registerReferenceProvider](cloudide_plugin_.languages.md#registerreferenceprovider)
- [registerRenameProvider](cloudide_plugin_.languages.md#registerrenameprovider)
- [registerSelectionRangeProvider](cloudide_plugin_.languages.md#registerselectionrangeprovider)
- [registerSignatureHelpProvider](cloudide_plugin_.languages.md#registersignaturehelpprovider)
- [registerTypeDefinitionProvider](cloudide_plugin_.languages.md#registertypedefinitionprovider)
- [registerWorkspaceSymbolProvider](cloudide_plugin_.languages.md#registerworkspacesymbolprovider)
- [setLanguageConfiguration](cloudide_plugin_.languages.md#setlanguageconfiguration)
- [setTextDocumentLanguage](cloudide_plugin_.languages.md#settextdocumentlanguage)

## Functions

### createDiagnosticCollection

▸ **createDiagnosticCollection**(`name?`): [`DiagnosticCollection`](../interfaces/cloudide_plugin_.DiagnosticCollection.md)

Create a diagnostics collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | The [name](#DiagnosticCollection.name) of the collection. |

#### Returns

[`DiagnosticCollection`](../interfaces/cloudide_plugin_.DiagnosticCollection.md)

A new diagnostic collection.

#### Defined in

[index.d.ts:8849](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8849)

___

### getDiagnostics

▸ **getDiagnostics**(`resource`): [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]

Get all diagnostics for a given resource. *Note* that this includes diagnostics from
all extensions but *not yet* from the task framework.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resource` | [`Uri`](../classes/cloudide_plugin_.Uri.md) | A resource |

#### Returns

[`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]

An array of [diagnostics](#Diagnostic) objects or an empty array.

#### Defined in

[index.d.ts:8833](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8833)

▸ **getDiagnostics**(): [[`Uri`](../classes/cloudide_plugin_.Uri.md), [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]][]

Get all diagnostics. *Note* that this includes diagnostics from
all extensions but *not yet* from the task framework.

#### Returns

[[`Uri`](../classes/cloudide_plugin_.Uri.md), [`Diagnostic`](../classes/cloudide_plugin_.Diagnostic.md)[]][]

An array of uri-diagnostics tuples or an empty array.

#### Defined in

[index.d.ts:8841](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8841)

___

### getLanguages

▸ **getLanguages**(): `PromiseLike`<`string`[]\>

Return the identifiers of all known languages.

#### Returns

`PromiseLike`<`string`[]\>

Promise resolving to an array of identifier strings.

#### Defined in

[index.d.ts:8766](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8766)

___

### match

▸ **match**(`selector`, `document`): `number`

Compute the match between a document [selector](#DocumentSelector) and a document. Values
greater than zero mean the selector matches the document.

A match is computed according to these rules:
1. When [`DocumentSelector`](#DocumentSelector) is an array, compute the match for each contained `DocumentFilter` or language identifier and take the maximum value.
2. A string will be desugared to become the `language`-part of a [`DocumentFilter`](#DocumentFilter), so `"fooLang"` is like `{ language: "fooLang" }`.
3. A [`DocumentFilter`](#DocumentFilter) will be matched against the document by comparing its parts with the document. The following rules apply:
 1. When the `DocumentFilter` is empty (`{}`) the result is `0`
 2. When `scheme`, `language`, or `pattern` are defined but one doesn’t match, the result is `0`
 3. Matching against `*` gives a score of `5`, matching via equality or via a glob-pattern gives a score of `10`
 4. The result is the maximum value of each match

Samples:
```js
// default document from disk (file-scheme)
doc.uri; //'file:///my/file.js'
doc.languageId; // 'javascript'
match('javascript', doc); // 10;
match({language: 'javascript'}, doc); // 10;
match({language: 'javascript', scheme: 'file'}, doc); // 10;
match('*', doc); // 5
match('fooLang', doc); // 0
match(['fooLang', '*'], doc); // 5

// virtual document, e.g. from git-index
doc.uri; // 'git:/my/file.js'
doc.languageId; // 'javascript'
match('javascript', doc); // 10;
match({language: 'javascript', scheme: 'git'}, doc); // 10;
match('*', doc); // 5
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A document selector. |
| `document` | [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) | A text document. |

#### Returns

`number`

A number `>0` when the selector matches and `0` when the selector does not match.

#### Defined in

[index.d.ts:8818](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8818)

___

### onDidChangeDiagnostics

▸ **onDidChangeDiagnostics**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DiagnosticChangeEvent`](../interfaces/cloudide_plugin_.DiagnosticChangeEvent.md)) => `any` | The listener function will be call when the event happens. |
| `thisArgs?` | `any` | The 'this' which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/cloudide_plugin_.Disposable.md)[] | An array to which a {{IDisposable}} will be added. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

a disposable to remove the listener again.

#### Defined in

[index.d.ts:2026](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L2026)

___

### registerCallHierarchyProvider

▸ **registerCallHierarchyProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a call hierarchy provider.

Multiple provider can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CallHierarchyProvider`](../interfaces/cloudide_plugin_.CallHierarchyProvider.md) | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9197](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9197)

___

### registerCodeActionsProvider

▸ **registerCodeActionsProvider**(`selector`, `provider`, `metadata?`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a code action provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CodeActionProvider`](../interfaces/cloudide_plugin_.CodeActionProvider.md) | A code action provider. |
| `metadata?` | [`CodeActionProviderMetadata`](../interfaces/cloudide_plugin_.CodeActionProviderMetadata.md) | Metadata about the kind of code actions the provider providers. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9024](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9024)

___

### registerCodeLensProvider

▸ **registerCodeLensProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a code lens provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CodeLensProvider`](../interfaces/cloudide_plugin_.CodeLensProvider.md)<[`CodeLens`](../classes/cloudide_plugin_.CodeLens.md)\> | A code lens provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9037](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9037)

___

### registerColorProvider

▸ **registerColorProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a color provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentColorProvider`](../interfaces/cloudide_plugin_.DocumentColorProvider.md) | A color provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9109](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9109)

___

### registerCompletionItemProvider

▸ **registerCompletionItemProvider**(`selector`, `provider`, `...triggerCharacters`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a completion provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and groups of equal score are sequentially asked for
completion items. The process stops when one or many providers of a group return a
result. A failing provider (rejected promise or exception) will not fail the whole
operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CompletionItemProvider`](../interfaces/cloudide_plugin_.CompletionItemProvider.md)<[`CompletionItem`](../classes/cloudide_plugin_.CompletionItem.md)\> | A completion provider. |
| `...triggerCharacters` | `string`[] | Trigger completion when the user types one of the characters, like `.` or `:`. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8874](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8874)

___

### registerDeclarationProvider

▸ **registerDeclarationProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a declaration provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DeclarationProvider`](../interfaces/cloudide_plugin_.DeclarationProvider.md) | A declaration provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8900](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8900)

___

### registerDefinitionProvider

▸ **registerDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DefinitionProvider`](../interfaces/cloudide_plugin_.DefinitionProvider.md) | A definition provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8887](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8887)

___

### registerDocumentFormattingEditProvider

▸ **registerDocumentFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a formatting provider for a document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentFormattingEditProvider`](../interfaces/cloudide_plugin_.DocumentFormattingEditProvider.md) | A document formatting edit provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8993](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8993)

___

### registerDocumentHighlightProvider

▸ **registerDocumentHighlightProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a document highlight provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and groups sequentially asked for document highlights.
The process stops when a provider returns a `non-falsy` or `non-failure` result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentHighlightProvider`](../interfaces/cloudide_plugin_.DocumentHighlightProvider.md) | A document highlight provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8980](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8980)

___

### registerDocumentLinkProvider

▸ **registerDocumentLinkProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a document link provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentLinkProvider`](../interfaces/cloudide_plugin_.DocumentLinkProvider.md)<[`DocumentLink`](../classes/cloudide_plugin_.DocumentLink.md)\> | A document link provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9070](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9070)

___

### registerDocumentRangeFormattingEditProvider

▸ **registerDocumentRangeFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a formatting provider for a document range.

*Note:* A document range provider is also a [document formatter](#DocumentFormattingEditProvider)
which means there is no need to [register](#registerDocumentFormattingEditProvider) a document
formatter when also registering a range provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentRangeFormattingEditProvider`](../interfaces/cloudide_plugin_.DocumentRangeFormattingEditProvider.md) | A document range formatting edit provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9010](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9010)

___

### registerDocumentRangeSemanticTokensProvider

▸ **registerDocumentRangeSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a semantic tokens provider for a document range.

*Note:* If a document has both a `DocumentSemanticTokensProvider` and a `DocumentRangeSemanticTokensProvider`,
the range provider will be invoked only initially, for the time in which the full document provider takes
to resolve the first request. Once the full document provider resolves the first request, the semantic tokens
provided via the range provider will be discarded and from that point forward, only the document provider
will be used.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentRangeSemanticTokensProvider`](../interfaces/cloudide_plugin_.DocumentRangeSemanticTokensProvider.md) | A document range semantic tokens provider. |
| `legend` | [`SemanticTokensLegend`](../classes/cloudide_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9184](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9184)

___

### registerDocumentSemanticTokensProvider

▸ **registerDocumentSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a semantic tokens provider for a whole document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentSemanticTokensProvider`](../interfaces/cloudide_plugin_.DocumentSemanticTokensProvider.md) | A document semantic tokens provider. |
| `legend` | [`SemanticTokensLegend`](../classes/cloudide_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9165](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9165)

___

### registerDocumentSymbolProvider

▸ **registerDocumentSymbolProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a document symbol provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentSymbolProvider`](../interfaces/cloudide_plugin_.DocumentSymbolProvider.md) | A document symbol provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9096](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9096)

___

### registerFoldingRangeProvider

▸ **registerFoldingRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a folding range provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged.
If multiple folding ranges start at the same position, only the range of the first registered provider is used.
If a folding range overlaps with an other range that has a smaller position, it is also ignored.

A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`FoldingRangeProvider`](../interfaces/cloudide_plugin_.FoldingRangeProvider.md) | A folding range provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9126](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9126)

___

### registerHoverProvider

▸ **registerHoverProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a hover provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`HoverProvider`](../interfaces/cloudide_plugin_.HoverProvider.md) | A hover provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8955](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8955)

___

### registerImplementationProvider

▸ **registerImplementationProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register an implementation provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`ImplementationProvider`](../interfaces/cloudide_plugin_.ImplementationProvider.md) | An implementation provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8942](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8942)

___

### registerOnTypeFormattingEditProvider

▸ **registerOnTypeFormattingEditProvider**(`selector`, `provider`, `firstTriggerCharacter`, `...moreTriggerCharacter`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a formatting provider that works on type. The provider is active when the user enables the setting `editor.formatOnType`.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`OnTypeFormattingEditProvider`](../interfaces/cloudide_plugin_.OnTypeFormattingEditProvider.md) | An on type formatting edit provider. |
| `firstTriggerCharacter` | `string` | A character on which formatting should be triggered, like `}`. |
| `...moreTriggerCharacter` | `string`[] | More trigger characters. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9052](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9052)

___

### registerReferenceProvider

▸ **registerReferenceProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a reference provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`ReferenceProvider`](../interfaces/cloudide_plugin_.ReferenceProvider.md) | A reference provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9083](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9083)

___

### registerRenameProvider

▸ **registerRenameProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a reference provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`RenameProvider`](../interfaces/cloudide_plugin_.RenameProvider.md) | A rename provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9152](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9152)

___

### registerSelectionRangeProvider

▸ **registerSelectionRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a selection range provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`SelectionRangeProvider`](../interfaces/cloudide_plugin_.SelectionRangeProvider.md) | A selection range provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:9139](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L9139)

___

### registerSignatureHelpProvider

▸ **registerSignatureHelpProvider**(`selector`, `provider`, `...triggerCharacters`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a signature help provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and called sequentially until a provider returns a
valid result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`SignatureHelpProvider`](../interfaces/cloudide_plugin_.SignatureHelpProvider.md) | A signature help provider. |
| `...triggerCharacters` | `string`[] | Trigger signature help when the user types one of the characters, like `,` or `(`. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8915](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8915)

▸ **registerSignatureHelpProvider**(`selector`, `provider`, `metadata`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) |
| `provider` | [`SignatureHelpProvider`](../interfaces/cloudide_plugin_.SignatureHelpProvider.md) |
| `metadata` | [`SignatureHelpProviderMetadata`](../interfaces/cloudide_plugin_.SignatureHelpProviderMetadata.md) |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

#### Defined in

[index.d.ts:8916](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8916)

___

### registerTypeDefinitionProvider

▸ **registerTypeDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a type definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_cloudide_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`TypeDefinitionProvider`](../interfaces/cloudide_plugin_.TypeDefinitionProvider.md) | A type definition provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8929](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8929)

___

### registerWorkspaceSymbolProvider

▸ **registerWorkspaceSymbolProvider**(`provider`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Register a workspace symbol provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`WorkspaceSymbolProvider`](../interfaces/cloudide_plugin_.WorkspaceSymbolProvider.md)<[`SymbolInformation`](../classes/cloudide_plugin_.SymbolInformation.md)\> | A workspace symbol provider. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:8967](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8967)

___

### setLanguageConfiguration

▸ **setLanguageConfiguration**(`language`, `configuration`): [`Disposable`](../classes/cloudide_plugin_.Disposable.md)

Set a [language configuration](#LanguageConfiguration) for a language.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `language` | `string` | A language identifier like `typescript`. |
| `configuration` | [`LanguageConfiguration`](../interfaces/cloudide_plugin_.LanguageConfiguration.md) | Language configuration. |

#### Returns

[`Disposable`](../classes/cloudide_plugin_.Disposable.md)

A [disposable](#Disposable) that unsets this configuration.

#### Defined in

[index.d.ts:8858](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8858)

___

### setTextDocumentLanguage

▸ **setTextDocumentLanguage**(`document`, `languageId`): `PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)\>

Set (and change) the [language](#TextDocument.languageId) that is associated
with the given document.

*Note* that calling this function will trigger the [`onDidCloseTextDocument`](#workspace.onDidCloseTextDocument) event
followed by the [`onDidOpenTextDocument`](#workspace.onDidOpenTextDocument) event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md) | The document which language is to be changed |
| `languageId` | `string` | The new language identifier. |

#### Returns

`PromiseLike`<[`TextDocument`](../interfaces/cloudide_plugin_.TextDocument.md)\>

A thenable that resolves with the updated document.

#### Defined in

[index.d.ts:8779](https://github.com/shuyaqian/cloudide-plugin-api/blob/26b31b9/index.d.ts#L8779)
