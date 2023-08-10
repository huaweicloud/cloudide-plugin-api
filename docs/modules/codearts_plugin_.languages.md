[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / languages

# Namespace: languages

["@codearts/plugin"](_codearts_plugin_.md).languages

Namespace for participating in language-specific editor [features](https://code.visualstudio.com/docs/editor/editingevolved),
like IntelliSense, code actions, diagnostics etc.

Many programming languages exist and there is huge variety in syntaxes, semantics, and paradigms. Despite that, features
like automatic word-completion, code navigation, or code checking have become popular across different tools for different
programming languages.

The editor provides an API that makes it simple to provide such common features by having all UI and actions already in place and
by allowing you to participate by providing data only. For instance, to contribute a hover all you have to do is provide a function
that can be called with a [TextDocument](../interfaces/codearts_plugin_.TextDocument.md) and a [Position](../classes/codearts_plugin_.Position.md) returning hover info. The rest, like tracking the
mouse, positioning the hover, keeping the hover stable etc. is taken care of by the editor.

```javascript
languages.registerHoverProvider('javascript', {
	provideHover(document, position, token) {
		return new Hover('I am a hover!');
	}
});
```

Registration is done using a [document selector](_codearts_plugin_.md#documentselector) which is either a language id, like `javascript` or
a more complex [filter](../interfaces/codearts_plugin_.DocumentFilter.md) like `{ language: 'typescript', scheme: 'file' }`. Matching a document against such
a selector will result in a [score](codearts_plugin_.languages.md#match) that is used to determine if and how a provider shall be used. When
scores are equal the provider that came last wins. For features that allow full arity, like [hover](codearts_plugin_.languages.md#registerhoverprovider),
the score is only checked to be `>0`, for other features, like [IntelliSense](codearts_plugin_.languages.md#registercompletionitemprovider) the
score is used for determining the order in which providers are asked to participate.

## Table of contents

### Functions

- [createDiagnosticCollection](codearts_plugin_.languages.md#creatediagnosticcollection)
- [createLanguageStatusItem](codearts_plugin_.languages.md#createlanguagestatusitem)
- [getDiagnostics](codearts_plugin_.languages.md#getdiagnostics)
- [getLanguages](codearts_plugin_.languages.md#getlanguages)
- [match](codearts_plugin_.languages.md#match)
- [onDidChangeDiagnostics](codearts_plugin_.languages.md#ondidchangediagnostics)
- [registerCallHierarchyProvider](codearts_plugin_.languages.md#registercallhierarchyprovider)
- [registerCodeActionsProvider](codearts_plugin_.languages.md#registercodeactionsprovider)
- [registerCodeLensProvider](codearts_plugin_.languages.md#registercodelensprovider)
- [registerColorProvider](codearts_plugin_.languages.md#registercolorprovider)
- [registerCompletionItemProvider](codearts_plugin_.languages.md#registercompletionitemprovider)
- [registerDeclarationProvider](codearts_plugin_.languages.md#registerdeclarationprovider)
- [registerDefinitionProvider](codearts_plugin_.languages.md#registerdefinitionprovider)
- [registerDocumentFormattingEditProvider](codearts_plugin_.languages.md#registerdocumentformattingeditprovider)
- [registerDocumentHighlightProvider](codearts_plugin_.languages.md#registerdocumenthighlightprovider)
- [registerDocumentLinkProvider](codearts_plugin_.languages.md#registerdocumentlinkprovider)
- [registerDocumentRangeFormattingEditProvider](codearts_plugin_.languages.md#registerdocumentrangeformattingeditprovider)
- [registerDocumentRangeSemanticTokensProvider](codearts_plugin_.languages.md#registerdocumentrangesemantictokensprovider)
- [registerDocumentSemanticTokensProvider](codearts_plugin_.languages.md#registerdocumentsemantictokensprovider)
- [registerDocumentSymbolProvider](codearts_plugin_.languages.md#registerdocumentsymbolprovider)
- [registerEvaluatableExpressionProvider](codearts_plugin_.languages.md#registerevaluatableexpressionprovider)
- [registerFoldingRangeProvider](codearts_plugin_.languages.md#registerfoldingrangeprovider)
- [registerHoverProvider](codearts_plugin_.languages.md#registerhoverprovider)
- [registerImplementationProvider](codearts_plugin_.languages.md#registerimplementationprovider)
- [registerInlayHintsProvider](codearts_plugin_.languages.md#registerinlayhintsprovider)
- [registerInlineCompletionItemProvider](codearts_plugin_.languages.md#registerinlinecompletionitemprovider)
- [registerInlineValuesProvider](codearts_plugin_.languages.md#registerinlinevaluesprovider)
- [registerLinkedEditingRangeProvider](codearts_plugin_.languages.md#registerlinkededitingrangeprovider)
- [registerOnTypeFormattingEditProvider](codearts_plugin_.languages.md#registerontypeformattingeditprovider)
- [registerReferenceProvider](codearts_plugin_.languages.md#registerreferenceprovider)
- [registerRenameProvider](codearts_plugin_.languages.md#registerrenameprovider)
- [registerSelectionRangeProvider](codearts_plugin_.languages.md#registerselectionrangeprovider)
- [registerSignatureHelpProvider](codearts_plugin_.languages.md#registersignaturehelpprovider)
- [registerTypeDefinitionProvider](codearts_plugin_.languages.md#registertypedefinitionprovider)
- [registerTypeHierarchyProvider](codearts_plugin_.languages.md#registertypehierarchyprovider)
- [registerWorkspaceSymbolProvider](codearts_plugin_.languages.md#registerworkspacesymbolprovider)
- [setLanguageConfiguration](codearts_plugin_.languages.md#setlanguageconfiguration)
- [setTextDocumentLanguage](codearts_plugin_.languages.md#settextdocumentlanguage)

## Functions

### createDiagnosticCollection

▸ **createDiagnosticCollection**(`name?`): [`DiagnosticCollection`](../interfaces/codearts_plugin_.DiagnosticCollection.md)

Create a diagnostics collection.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` | The [name](../interfaces/codearts_plugin_.DiagnosticCollection.md#name) of the collection. |

#### Returns

[`DiagnosticCollection`](../interfaces/codearts_plugin_.DiagnosticCollection.md)

A new diagnostic collection.

#### Defined in

[index.d.ts:13317](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13317)

___

### createLanguageStatusItem

▸ **createLanguageStatusItem**(`id`, `selector`): [`LanguageStatusItem`](../interfaces/codearts_plugin_.LanguageStatusItem.md)

Creates a new [language status item](../interfaces/codearts_plugin_.LanguageStatusItem.md).

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The identifier of the item. |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | The document selector that defines for what editors the item shows. |

#### Returns

[`LanguageStatusItem`](../interfaces/codearts_plugin_.LanguageStatusItem.md)

#### Defined in

[index.d.ts:13325](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13325)

___

### getDiagnostics

▸ **getDiagnostics**(`resource`): [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

Get all diagnostics for a given resource.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resource` | [`Uri`](../classes/codearts_plugin_.Uri.md) | A resource |

#### Returns

[`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

An array of [diagnostics](../classes/codearts_plugin_.Diagnostic.md) objects or an empty array.

#### Defined in

[index.d.ts:13302](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13302)

▸ **getDiagnostics**(): [[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

Get all diagnostics.

#### Returns

[[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

An array of uri-diagnostics tuples or an empty array.

#### Defined in

[index.d.ts:13309](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13309)

___

### getLanguages

▸ **getLanguages**(): [`Thenable`](../interfaces/Thenable.md)<`string`[]\>

Return the identifiers of all known languages.

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[]\>

Promise resolving to an array of identifier strings.

#### Defined in

[index.d.ts:13228](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13228)

___

### match

▸ **match**(`selector`, `document`): `number`

Compute the match between a document [selector](_codearts_plugin_.md#documentselector) and a document. Values
greater than zero mean the selector matches the document.

A match is computed according to these rules:
1. When [`DocumentSelector`](_codearts_plugin_.md#documentselector) is an array, compute the match for each contained `DocumentFilter` or language identifier and take the maximum value.
2. A string will be desugared to become the `language`-part of a [`DocumentFilter`](../interfaces/codearts_plugin_.DocumentFilter.md), so `"fooLang"` is like `{ language: "fooLang" }`.
3. A [`DocumentFilter`](../interfaces/codearts_plugin_.DocumentFilter.md) will be matched against the document by comparing its parts with the document. The following rules apply:
   1. When the `DocumentFilter` is empty (`{}`) the result is `0`
   2. When `scheme`, `language`, `pattern`, or `notebook` are defined but one doesn't match, the result is `0`
   3. Matching against `*` gives a score of `5`, matching via equality or via a glob-pattern gives a score of `10`
   4. The result is the maximum value of each match

Samples:
```js
// default document from disk (file-scheme)
doc.uri; //'file:///my/file.js'
doc.languageId; // 'javascript'
match('javascript', doc); // 10;
match({ language: 'javascript' }, doc); // 10;
match({ language: 'javascript', scheme: 'file' }, doc); // 10;
match('*', doc); // 5
match('fooLang', doc); // 0
match(['fooLang', '*'], doc); // 5

// virtual document, e.g. from git-index
doc.uri; // 'git:/my/file.js'
doc.languageId; // 'javascript'
match('javascript', doc); // 10;
match({ language: 'javascript', scheme: 'git' }, doc); // 10;
match('*', doc); // 5

// notebook cell document
doc.uri; // `vscode-notebook-cell:///my/notebook.ipynb#gl65s2pmha`;
doc.languageId; // 'python'
match({ notebookType: 'jupyter-notebook' }, doc) // 10
match({ notebookType: 'fooNotebook', language: 'python' }, doc) // 0
match({ language: 'python' }, doc) // 10
match({ notebookType: '*' }, doc) // 5
```

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A document selector. |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) | A text document. |

#### Returns

`number`

A number `>0` when the selector matches and `0` when the selector does not match.

#### Defined in

[index.d.ts:13288](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13288)

___

### onDidChangeDiagnostics

▸ **onDidChangeDiagnostics**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

A function that represents an event to which you subscribe by calling it with
a listener function as argument.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `listener` | (`e`: [`DiagnosticChangeEvent`](../interfaces/codearts_plugin_.DiagnosticChangeEvent.md)) => `any` | The listener function will be called when the event happens. |
| `thisArgs?` | `any` | The `this`-argument which will be used when calling the event listener. |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] | An array to which a [Disposable](../classes/codearts_plugin_.Disposable.md) will be added. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A disposable which unsubscribes the event listener.

#### Defined in

[index.d.ts:1603](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L1603)

___

### registerCallHierarchyProvider

▸ **registerCallHierarchyProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a call hierarchy provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CallHierarchyProvider`](../interfaces/codearts_plugin_.CallHierarchyProvider.md) | A call hierarchy provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13714](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13714)

___

### registerCodeActionsProvider

▸ **registerCodeActionsProvider**(`selector`, `provider`, `metadata?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a code action provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CodeActionProvider`](../interfaces/codearts_plugin_.CodeActionProvider.md)<[`CodeAction`](../classes/codearts_plugin_.CodeAction.md)\> | A code action provider. |
| `metadata?` | [`CodeActionProviderMetadata`](../interfaces/codearts_plugin_.CodeActionProviderMetadata.md) | Metadata about the kind of code actions the provider provides. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13373](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13373)

___

### registerCodeLensProvider

▸ **registerCodeLensProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a code lens provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CodeLensProvider`](../interfaces/codearts_plugin_.CodeLensProvider.md)<[`CodeLens`](../classes/codearts_plugin_.CodeLens.md)\> | A code lens provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13387](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13387)

___

### registerColorProvider

▸ **registerColorProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a color provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentColorProvider`](../interfaces/codearts_plugin_.DocumentColorProvider.md) | A color provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13662](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13662)

___

### registerCompletionItemProvider

▸ **registerCompletionItemProvider**(`selector`, `provider`, ...`triggerCharacters`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a completion provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and groups of equal score are sequentially asked for
completion items. The process stops when one or many providers of a group return a
result. A failing provider (rejected promise or exception) will not fail the whole
operation.

A completion item provider can be associated with a set of `triggerCharacters`. When trigger
characters are being typed, completions are requested but only from providers that registered
the typed character. Because of that trigger characters should be different than [word characters](../interfaces/codearts_plugin_.LanguageConfiguration.md#wordpattern),
a common trigger character is `.` to trigger member completions.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`CompletionItemProvider`](../interfaces/codearts_plugin_.CompletionItemProvider.md)<[`CompletionItem`](../classes/codearts_plugin_.CompletionItem.md)\> | A completion provider. |
| `...triggerCharacters` | `string`[] | Trigger completion when the user types one of the characters. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13346](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13346)

___

### registerDeclarationProvider

▸ **registerDeclarationProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a declaration provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DeclarationProvider`](../interfaces/codearts_plugin_.DeclarationProvider.md) | A declaration provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13438](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13438)

___

### registerDefinitionProvider

▸ **registerDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DefinitionProvider`](../interfaces/codearts_plugin_.DefinitionProvider.md) | A definition provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13399](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13399)

___

### registerDocumentFormattingEditProvider

▸ **registerDocumentFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a formatting provider for a document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentFormattingEditProvider`](../interfaces/codearts_plugin_.DocumentFormattingEditProvider.md) | A document formatting edit provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13588](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13588)

___

### registerDocumentHighlightProvider

▸ **registerDocumentHighlightProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a document highlight provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and groups sequentially asked for document highlights.
The process stops when a provider returns a `non-falsy` or `non-failure` result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentHighlightProvider`](../interfaces/codearts_plugin_.DocumentHighlightProvider.md) | A document highlight provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13491](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13491)

___

### registerDocumentLinkProvider

▸ **registerDocumentLinkProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a document link provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentLinkProvider`](../interfaces/codearts_plugin_.DocumentLinkProvider.md)<[`DocumentLink`](../classes/codearts_plugin_.DocumentLink.md)\> | A document link provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13649](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13649)

___

### registerDocumentRangeFormattingEditProvider

▸ **registerDocumentRangeFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a formatting provider for a document range.

*Note:* A document range provider is also a [document formatter](../interfaces/codearts_plugin_.DocumentFormattingEditProvider.md)
which means there is no need to [register](codearts_plugin_.languages.md#registerdocumentformattingeditprovider) a document
formatter when also registering a range provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentRangeFormattingEditProvider`](../interfaces/codearts_plugin_.DocumentRangeFormattingEditProvider.md) | A document range formatting edit provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13605](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13605)

___

### registerDocumentRangeSemanticTokensProvider

▸ **registerDocumentRangeSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a semantic tokens provider for a document range.

*Note:* If a document has both a `DocumentSemanticTokensProvider` and a `DocumentRangeSemanticTokensProvider`,
the range provider will be invoked only initially, for the time in which the full document provider takes
to resolve the first request. Once the full document provider resolves the first request, the semantic tokens
provided via the range provider will be discarded and from that point forward, only the document provider
will be used.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentRangeSemanticTokensProvider`](../interfaces/codearts_plugin_.DocumentRangeSemanticTokensProvider.md) | A document range semantic tokens provider. |
| `legend` | [`SemanticTokensLegend`](../classes/codearts_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13575](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13575)

___

### registerDocumentSemanticTokensProvider

▸ **registerDocumentSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a semantic tokens provider for a whole document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentSemanticTokensProvider`](../interfaces/codearts_plugin_.DocumentSemanticTokensProvider.md) | A document semantic tokens provider. |
| `legend` | [`SemanticTokensLegend`](../classes/codearts_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13556](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13556)

___

### registerDocumentSymbolProvider

▸ **registerDocumentSymbolProvider**(`selector`, `provider`, `metaData?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a document symbol provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`DocumentSymbolProvider`](../interfaces/codearts_plugin_.DocumentSymbolProvider.md) | A document symbol provider. |
| `metaData?` | [`DocumentSymbolProviderMetadata`](../interfaces/codearts_plugin_.DocumentSymbolProviderMetadata.md) | metadata about the provider |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13505](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13505)

___

### registerEvaluatableExpressionProvider

▸ **registerEvaluatableExpressionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a provider that locates evaluatable expressions in text documents.
The editor will evaluate the expression in the active debug session and will show the result in the debug hover.

If multiple providers are registered for a language an arbitrary provider will be used.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`EvaluatableExpressionProvider`](../interfaces/codearts_plugin_.EvaluatableExpressionProvider.md) | An evaluatable expression provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13463](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13463)

___

### registerFoldingRangeProvider

▸ **registerFoldingRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

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
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`FoldingRangeProvider`](../interfaces/codearts_plugin_.FoldingRangeProvider.md) | A folding range provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13692](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13692)

___

### registerHoverProvider

▸ **registerHoverProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a hover provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`HoverProvider`](../interfaces/codearts_plugin_.HoverProvider.md) | A hover provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13451](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13451)

___

### registerImplementationProvider

▸ **registerImplementationProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register an implementation provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`ImplementationProvider`](../interfaces/codearts_plugin_.ImplementationProvider.md) | An implementation provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13412](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13412)

___

### registerInlayHintsProvider

▸ **registerInlayHintsProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a inlay hints provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`InlayHintsProvider`](../interfaces/codearts_plugin_.InlayHintsProvider.md)<[`InlayHint`](../classes/codearts_plugin_.InlayHint.md)\> | An inlay hints provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13675](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13675)

___

### registerInlineCompletionItemProvider

▸ **registerInlineCompletionItemProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Registers an inline completion provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`InlineCompletionItemProvider`](../interfaces/codearts_plugin_.InlineCompletionItemProvider.md) | An inline completion provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13359](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13359)

___

### registerInlineValuesProvider

▸ **registerInlineValuesProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a provider that returns data for the debugger's 'inline value' feature.
Whenever the generic debugger has stopped in a source file, providers registered for the language of the file
are called to return textual data that will be shown in the editor at the end of lines.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`InlineValuesProvider`](../interfaces/codearts_plugin_.InlineValuesProvider.md) | An inline values provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13478](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13478)

___

### registerLinkedEditingRangeProvider

▸ **registerLinkedEditingRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a linked editing range provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider that has a result is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`LinkedEditingRangeProvider`](../interfaces/codearts_plugin_.LinkedEditingRangeProvider.md) | A linked editing range provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13736](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13736)

___

### registerOnTypeFormattingEditProvider

▸ **registerOnTypeFormattingEditProvider**(`selector`, `provider`, `firstTriggerCharacter`, ...`moreTriggerCharacter`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a formatting provider that works on type. The provider is active when the user enables the setting `editor.formatOnType`.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`OnTypeFormattingEditProvider`](../interfaces/codearts_plugin_.OnTypeFormattingEditProvider.md) | An on type formatting edit provider. |
| `firstTriggerCharacter` | `string` | A character on which formatting should be triggered, like `}`. |
| `...moreTriggerCharacter` | `string`[] | More trigger characters. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13620](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13620)

___

### registerReferenceProvider

▸ **registerReferenceProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a reference provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`ReferenceProvider`](../interfaces/codearts_plugin_.ReferenceProvider.md) | A reference provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13530](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13530)

___

### registerRenameProvider

▸ **registerRenameProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a rename provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and asked in sequence. The first provider producing a result
defines the result of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`RenameProvider`](../interfaces/codearts_plugin_.RenameProvider.md) | A rename provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13543](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13543)

___

### registerSelectionRangeProvider

▸ **registerSelectionRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a selection range provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`SelectionRangeProvider`](../interfaces/codearts_plugin_.SelectionRangeProvider.md) | A selection range provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13705](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13705)

___

### registerSignatureHelpProvider

▸ **registerSignatureHelpProvider**(`selector`, `provider`, ...`triggerCharacters`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a signature help provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](codearts_plugin_.languages.md#match) and called sequentially until a provider returns a
valid result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`SignatureHelpProvider`](../interfaces/codearts_plugin_.SignatureHelpProvider.md) | A signature help provider. |
| `...triggerCharacters` | `string`[] | Trigger signature help when the user types one of the characters, like `,` or `(`. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13635](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13635)

▸ **registerSignatureHelpProvider**(`selector`, `provider`, `metadata`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |
| `provider` | [`SignatureHelpProvider`](../interfaces/codearts_plugin_.SignatureHelpProvider.md) |
| `metadata` | [`SignatureHelpProviderMetadata`](../interfaces/codearts_plugin_.SignatureHelpProviderMetadata.md) |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:13636](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13636)

___

### registerTypeDefinitionProvider

▸ **registerTypeDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a type definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`TypeDefinitionProvider`](../interfaces/codearts_plugin_.TypeDefinitionProvider.md) | A type definition provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13425](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13425)

___

### registerTypeHierarchyProvider

▸ **registerTypeHierarchyProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a type hierarchy provider.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
| `provider` | [`TypeHierarchyProvider`](../interfaces/codearts_plugin_.TypeHierarchyProvider.md) | A type hierarchy provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13723](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13723)

___

### registerWorkspaceSymbolProvider

▸ **registerWorkspaceSymbolProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Register a workspace symbol provider.

Multiple providers can be registered. In that case providers are asked in parallel and
the results are merged. A failing provider (rejected promise or exception) will not cause
a failure of the whole operation.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`WorkspaceSymbolProvider`](../interfaces/codearts_plugin_.WorkspaceSymbolProvider.md)<[`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)\> | A workspace symbol provider. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unregisters this provider when being disposed.

#### Defined in

[index.d.ts:13517](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13517)

___

### setLanguageConfiguration

▸ **setLanguageConfiguration**(`language`, `configuration`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

Set a [language configuration](../interfaces/codearts_plugin_.LanguageConfiguration.md) for a language.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `language` | `string` | A language identifier like `typescript`. |
| `configuration` | [`LanguageConfiguration`](../interfaces/codearts_plugin_.LanguageConfiguration.md) | Language configuration. |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

A [Disposable](../classes/codearts_plugin_.Disposable.md) that unsets this configuration.

#### Defined in

[index.d.ts:13745](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13745)

___

### setTextDocumentLanguage

▸ **setTextDocumentLanguage**(`document`, `languageId`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

Set (and change) the [language](../interfaces/codearts_plugin_.TextDocument.md#languageid) that is associated
with the given document.

*Note* that calling this function will trigger the [`onDidCloseTextDocument`](codearts_plugin_.workspace.md#ondidclosetextdocument) event
followed by the [`onDidOpenTextDocument`](codearts_plugin_.workspace.md#ondidopentextdocument) event.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) | The document which language is to be changed |
| `languageId` | `string` | The new language identifier. |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

A thenable that resolves with the updated document.

#### Defined in

[index.d.ts:13241](https://github.com/shuyaqian/cloudide-plugin-api/blob/3fbdd11/index.d.ts#L13241)
