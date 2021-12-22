**[@cloudide/plugin](../README.md)**

> [Globals](../README.md) / ["index.d"](_index_d_.md) / ["plugin"](_index_d_._plugin_.md) / languages

# Namespace: languages

Namespace for participating in language-specific editor [features](https://code.visualstudio.com/docs/editor/editingevolved),
like IntelliSense, code actions, diagnostics etc.

Many programming languages exist and there is huge variety in syntaxes, semantics, and paradigms. Despite that, features
like automatic word-completion, code navigation, or code checking have become popular across different tools for different
programming languages.

The editor provides an API that makes it simple to provide such common features by having all UI and actions already in place and
by allowing you to participate by providing data only. For instance, to contribute a hover all you have to do is provide a function
that can be called with a [TextDocument](#TextDocument) and a [Position](#Position) returning hover info. The rest, like tracking the
mouse, positioning the hover, keeping the hover stable etc. is taken care of by the editor.

```javascript
languages.registerHoverProvider('javascript', {
	provideHover(document, position, token) {
		return new Hover('I am a hover!');
	}
});
```

Registration is done using a [document selector](#DocumentSelector) which is either a language id, like `javascript` or
a more complex [filter](#DocumentFilter) like `{ language: 'typescript', scheme: 'file' }`. Matching a document against such
a selector will result in a [score](#languages.match) that is used to determine if and how a provider shall be used. When
scores are equal the provider that came last wins. For features that allow full arity, like [hover](#languages.registerHoverProvider),
the score is only checked to be `>0`, for other features, like [IntelliSense](#languages.registerCompletionItemProvider) the
score is used for determining the order in which providers are asked to participate.

## Index

### Variables

* [onDidChangeDiagnostics](_index_d_._plugin_.languages.md#ondidchangediagnostics)

### Functions

* [createDiagnosticCollection](_index_d_._plugin_.languages.md#creatediagnosticcollection)
* [getDiagnostics](_index_d_._plugin_.languages.md#getdiagnostics)
* [getLanguages](_index_d_._plugin_.languages.md#getlanguages)
* [match](_index_d_._plugin_.languages.md#match)
* [registerCallHierarchyProvider](_index_d_._plugin_.languages.md#registercallhierarchyprovider)
* [registerCodeActionsProvider](_index_d_._plugin_.languages.md#registercodeactionsprovider)
* [registerCodeLensProvider](_index_d_._plugin_.languages.md#registercodelensprovider)
* [registerColorProvider](_index_d_._plugin_.languages.md#registercolorprovider)
* [registerCompletionItemProvider](_index_d_._plugin_.languages.md#registercompletionitemprovider)
* [registerDeclarationProvider](_index_d_._plugin_.languages.md#registerdeclarationprovider)
* [registerDefinitionProvider](_index_d_._plugin_.languages.md#registerdefinitionprovider)
* [registerDocumentFormattingEditProvider](_index_d_._plugin_.languages.md#registerdocumentformattingeditprovider)
* [registerDocumentHighlightProvider](_index_d_._plugin_.languages.md#registerdocumenthighlightprovider)
* [registerDocumentLinkProvider](_index_d_._plugin_.languages.md#registerdocumentlinkprovider)
* [registerDocumentRangeFormattingEditProvider](_index_d_._plugin_.languages.md#registerdocumentrangeformattingeditprovider)
* [registerDocumentRangeSemanticTokensProvider](_index_d_._plugin_.languages.md#registerdocumentrangesemantictokensprovider)
* [registerDocumentSemanticTokensProvider](_index_d_._plugin_.languages.md#registerdocumentsemantictokensprovider)
* [registerDocumentSymbolProvider](_index_d_._plugin_.languages.md#registerdocumentsymbolprovider)
* [registerEvaluatableExpressionProvider](_index_d_._plugin_.languages.md#registerevaluatableexpressionprovider)
* [registerFoldingRangeProvider](_index_d_._plugin_.languages.md#registerfoldingrangeprovider)
* [registerHoverProvider](_index_d_._plugin_.languages.md#registerhoverprovider)
* [registerImplementationProvider](_index_d_._plugin_.languages.md#registerimplementationprovider)
* [registerLinkedEditingRangeProvider](_index_d_._plugin_.languages.md#registerlinkededitingrangeprovider)
* [registerOnTypeFormattingEditProvider](_index_d_._plugin_.languages.md#registerontypeformattingeditprovider)
* [registerReferenceProvider](_index_d_._plugin_.languages.md#registerreferenceprovider)
* [registerRenameProvider](_index_d_._plugin_.languages.md#registerrenameprovider)
* [registerSelectionRangeProvider](_index_d_._plugin_.languages.md#registerselectionrangeprovider)
* [registerSignatureHelpProvider](_index_d_._plugin_.languages.md#registersignaturehelpprovider)
* [registerTypeDefinitionProvider](_index_d_._plugin_.languages.md#registertypedefinitionprovider)
* [registerWorkspaceSymbolProvider](_index_d_._plugin_.languages.md#registerworkspacesymbolprovider)
* [setLanguageConfiguration](_index_d_._plugin_.languages.md#setlanguageconfiguration)
* [setTextDocumentLanguage](_index_d_._plugin_.languages.md#settextdocumentlanguage)

## Variables

### onDidChangeDiagnostics

• `Const` **onDidChangeDiagnostics**: [Event](../interfaces/_index_d_._plugin_.event.md)\<[DiagnosticChangeEvent](../interfaces/_index_d_._plugin_.diagnosticchangeevent.md)>

*Defined in [index.d.ts:10843](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10843)*

An [event](#Event) which fires when the global set of diagnostics changes. This is
newly added and removed diagnostics.

## Functions

### createDiagnosticCollection

▸ **createDiagnosticCollection**(`name?`: string): [DiagnosticCollection](../interfaces/_index_d_._plugin_.diagnosticcollection.md)

*Defined in [index.d.ts:10866](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10866)*

Create a diagnostics collection.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`name?` | string | The [name](#DiagnosticCollection.name) of the collection. |

**Returns:** [DiagnosticCollection](../interfaces/_index_d_._plugin_.diagnosticcollection.md)

A new diagnostic collection.

___

### getDiagnostics

▸ **getDiagnostics**(`resource`: [Uri](../classes/_index_d_._plugin_.uri.md)): [Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)[]

*Defined in [index.d.ts:10851](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10851)*

Get all diagnostics for a given resource.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`resource` | [Uri](../classes/_index_d_._plugin_.uri.md) | A resource |

**Returns:** [Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)[]

An array of [diagnostics](#Diagnostic) objects or an empty array.

▸ **getDiagnostics**(): [[Uri](../classes/_index_d_._plugin_.uri.md), [Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)[]][]

*Defined in [index.d.ts:10858](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10858)*

Get all diagnostics.

**Returns:** [[Uri](../classes/_index_d_._plugin_.uri.md), [Diagnostic](../classes/_index_d_._plugin_.diagnostic.md)[]][]

An array of uri-diagnostics tuples or an empty array.

___

### getLanguages

▸ **getLanguages**(): [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>

*Defined in [index.d.ts:10785](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10785)*

Return the identifiers of all known languages.

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<string[]>

Promise resolving to an array of identifier strings.

___

### match

▸ **match**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `document`: [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)): number

*Defined in [index.d.ts:10837](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10837)*

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

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A document selector. |
`document` | [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md) | A text document. |

**Returns:** number

A number `>0` when the selector matches and `0` when the selector does not match.

___

### registerCallHierarchyProvider

▸ **registerCallHierarchyProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [CallHierarchyProvider](../interfaces/_index_d_._plugin_.callhierarchyprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11214](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11214)*

Register a call hierarchy provider.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [CallHierarchyProvider](../interfaces/_index_d_._plugin_.callhierarchyprovider.md) | A call hierarchy provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerCodeActionsProvider

▸ **registerCodeActionsProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [CodeActionProvider](../interfaces/_index_d_._plugin_.codeactionprovider.md), `metadata?`: [CodeActionProviderMetadata](../interfaces/_index_d_._plugin_.codeactionprovidermetadata.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10901](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10901)*

Register a code action provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [CodeActionProvider](../interfaces/_index_d_._plugin_.codeactionprovider.md) | A code action provider. |
`metadata?` | [CodeActionProviderMetadata](../interfaces/_index_d_._plugin_.codeactionprovidermetadata.md) | Metadata about the kind of code actions the provider provides. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerCodeLensProvider

▸ **registerCodeLensProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [CodeLensProvider](../interfaces/_index_d_._plugin_.codelensprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10914](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10914)*

Register a code lens provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [CodeLensProvider](../interfaces/_index_d_._plugin_.codelensprovider.md) | A code lens provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerColorProvider

▸ **registerColorProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentColorProvider](../interfaces/_index_d_._plugin_.documentcolorprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11175](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11175)*

Register a color provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentColorProvider](../interfaces/_index_d_._plugin_.documentcolorprovider.md) | A color provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerCompletionItemProvider

▸ **registerCompletionItemProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [CompletionItemProvider](../interfaces/_index_d_._plugin_.completionitemprovider.md), ...`triggerCharacters`: string[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10887](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10887)*

Register a completion provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and groups of equal score are sequentially asked for
completion items. The process stops when one or many providers of a group return a
result. A failing provider (rejected promise or exception) will not fail the whole
operation.

A completion item provider can be associated with a set of `triggerCharacters`. When trigger
characters are being typed, completions are requested but only from providers that registered
the typed character. Because of that trigger characters should be different than [word characters](#LanguageConfiguration.wordPattern),
a common trigger character is `.` to trigger member completions.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [CompletionItemProvider](../interfaces/_index_d_._plugin_.completionitemprovider.md) | A completion provider. |
`...triggerCharacters` | string[] | Trigger completion when the user types one of the characters. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDeclarationProvider

▸ **registerDeclarationProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DeclarationProvider](../interfaces/_index_d_._plugin_.declarationprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10966](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10966)*

Register a declaration provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DeclarationProvider](../interfaces/_index_d_._plugin_.declarationprovider.md) | A declaration provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDefinitionProvider

▸ **registerDefinitionProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DefinitionProvider](../interfaces/_index_d_._plugin_.definitionprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10927](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10927)*

Register a definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DefinitionProvider](../interfaces/_index_d_._plugin_.definitionprovider.md) | A definition provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentFormattingEditProvider

▸ **registerDocumentFormattingEditProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentFormattingEditProvider](../interfaces/_index_d_._plugin_.documentformattingeditprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11101](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11101)*

Register a formatting provider for a document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentFormattingEditProvider](../interfaces/_index_d_._plugin_.documentformattingeditprovider.md) | A document formatting edit provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentHighlightProvider

▸ **registerDocumentHighlightProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentHighlightProvider](../interfaces/_index_d_._plugin_.documenthighlightprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11004](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11004)*

Register a document highlight provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and groups sequentially asked for document highlights.
The process stops when a provider returns a `non-falsy` or `non-failure` result.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentHighlightProvider](../interfaces/_index_d_._plugin_.documenthighlightprovider.md) | A document highlight provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentLinkProvider

▸ **registerDocumentLinkProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentLinkProvider](../interfaces/_index_d_._plugin_.documentlinkprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11162](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11162)*

Register a document link provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentLinkProvider](../interfaces/_index_d_._plugin_.documentlinkprovider.md) | A document link provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentRangeFormattingEditProvider

▸ **registerDocumentRangeFormattingEditProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentRangeFormattingEditProvider](../interfaces/_index_d_._plugin_.documentrangeformattingeditprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11118](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11118)*

Register a formatting provider for a document range.

*Note:* A document range provider is also a [document formatter](#DocumentFormattingEditProvider)
which means there is no need to [register](#languages.registerDocumentFormattingEditProvider) a document
formatter when also registering a range provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentRangeFormattingEditProvider](../interfaces/_index_d_._plugin_.documentrangeformattingeditprovider.md) | A document range formatting edit provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentRangeSemanticTokensProvider

▸ **registerDocumentRangeSemanticTokensProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentRangeSemanticTokensProvider](../interfaces/_index_d_._plugin_.documentrangesemantictokensprovider.md), `legend`: [SemanticTokensLegend](../classes/_index_d_._plugin_.semantictokenslegend.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11088](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11088)*

Register a semantic tokens provider for a document range.

*Note:* If a document has both a `DocumentSemanticTokensProvider` and a `DocumentRangeSemanticTokensProvider`,
the range provider will be invoked only initially, for the time in which the full document provider takes
to resolve the first request. Once the full document provider resolves the first request, the semantic tokens
provided via the range provider will be discarded and from that point forward, only the document provider
will be used.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentRangeSemanticTokensProvider](../interfaces/_index_d_._plugin_.documentrangesemantictokensprovider.md) | A document range semantic tokens provider. |
`legend` | [SemanticTokensLegend](../classes/_index_d_._plugin_.semantictokenslegend.md) | - |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentSemanticTokensProvider

▸ **registerDocumentSemanticTokensProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentSemanticTokensProvider](../interfaces/_index_d_._plugin_.documentsemantictokensprovider.md), `legend`: [SemanticTokensLegend](../classes/_index_d_._plugin_.semantictokenslegend.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11069](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11069)*

Register a semantic tokens provider for a whole document.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentSemanticTokensProvider](../interfaces/_index_d_._plugin_.documentsemantictokensprovider.md) | A document semantic tokens provider. |
`legend` | [SemanticTokensLegend](../classes/_index_d_._plugin_.semantictokenslegend.md) | - |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerDocumentSymbolProvider

▸ **registerDocumentSymbolProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [DocumentSymbolProvider](../interfaces/_index_d_._plugin_.documentsymbolprovider.md), `metaData?`: [DocumentSymbolProviderMetadata](../interfaces/_index_d_._plugin_.documentsymbolprovidermetadata.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11018](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11018)*

Register a document symbol provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [DocumentSymbolProvider](../interfaces/_index_d_._plugin_.documentsymbolprovider.md) | A document symbol provider. |
`metaData?` | [DocumentSymbolProviderMetadata](../interfaces/_index_d_._plugin_.documentsymbolprovidermetadata.md) | metadata about the provider |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerEvaluatableExpressionProvider

▸ **registerEvaluatableExpressionProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [EvaluatableExpressionProvider](../interfaces/_index_d_._plugin_.evaluatableexpressionprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10991](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10991)*

Register a provider that locates evaluatable expressions in text documents.
VS Code will evaluate the expression in the active debug session and will show the result in the debug hover.

If multiple providers are registered for a language an arbitrary provider will be used.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [EvaluatableExpressionProvider](../interfaces/_index_d_._plugin_.evaluatableexpressionprovider.md) | An evaluatable expression provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerFoldingRangeProvider

▸ **registerFoldingRangeProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [FoldingRangeProvider](../interfaces/_index_d_._plugin_.foldingrangeprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11192](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11192)*

Register a folding range provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged.
If multiple folding ranges start at the same position, only the range of the first registered provider is used.
If a folding range overlaps with an other range that has a smaller position, it is also ignored.

A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [FoldingRangeProvider](../interfaces/_index_d_._plugin_.foldingrangeprovider.md) | A folding range provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerHoverProvider

▸ **registerHoverProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [HoverProvider](../interfaces/_index_d_._plugin_.hoverprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10979](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10979)*

Register a hover provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [HoverProvider](../interfaces/_index_d_._plugin_.hoverprovider.md) | A hover provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerImplementationProvider

▸ **registerImplementationProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [ImplementationProvider](../interfaces/_index_d_._plugin_.implementationprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10940](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10940)*

Register an implementation provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [ImplementationProvider](../interfaces/_index_d_._plugin_.implementationprovider.md) | An implementation provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerLinkedEditingRangeProvider

▸ **registerLinkedEditingRangeProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [LinkedEditingRangeProvider](../interfaces/_index_d_._plugin_.linkededitingrangeprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11227](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11227)*

Register a linked editing range provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider that has a result is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [LinkedEditingRangeProvider](../interfaces/_index_d_._plugin_.linkededitingrangeprovider.md) | A linked editing range provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerOnTypeFormattingEditProvider

▸ **registerOnTypeFormattingEditProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [OnTypeFormattingEditProvider](../interfaces/_index_d_._plugin_.ontypeformattingeditprovider.md), `firstTriggerCharacter`: string, ...`moreTriggerCharacter`: string[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11133](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11133)*

Register a formatting provider that works on type. The provider is active when the user enables the setting `editor.formatOnType`.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and the best-matching provider is used. Failure
of the selected provider will cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [OnTypeFormattingEditProvider](../interfaces/_index_d_._plugin_.ontypeformattingeditprovider.md) | An on type formatting edit provider. |
`firstTriggerCharacter` | string | A character on which formatting should be triggered, like `}`. |
`...moreTriggerCharacter` | string[] | More trigger characters. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerReferenceProvider

▸ **registerReferenceProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [ReferenceProvider](../interfaces/_index_d_._plugin_.referenceprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11043](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11043)*

Register a reference provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [ReferenceProvider](../interfaces/_index_d_._plugin_.referenceprovider.md) | A reference provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerRenameProvider

▸ **registerRenameProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [RenameProvider](../interfaces/_index_d_._plugin_.renameprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11056](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11056)*

Register a rename provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and asked in sequence. The first provider producing a result
defines the result of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [RenameProvider](../interfaces/_index_d_._plugin_.renameprovider.md) | A rename provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerSelectionRangeProvider

▸ **registerSelectionRangeProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [SelectionRangeProvider](../interfaces/_index_d_._plugin_.selectionrangeprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11205](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11205)*

Register a selection range provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [SelectionRangeProvider](../interfaces/_index_d_._plugin_.selectionrangeprovider.md) | A selection range provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerSignatureHelpProvider

▸ **registerSignatureHelpProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [SignatureHelpProvider](../interfaces/_index_d_._plugin_.signaturehelpprovider.md), ...`triggerCharacters`: string[]): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11148](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11148)*

Register a signature help provider.

Multiple providers can be registered for a language. In that case providers are sorted
by their [score](#languages.match) and called sequentially until a provider returns a
valid result.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [SignatureHelpProvider](../interfaces/_index_d_._plugin_.signaturehelpprovider.md) | A signature help provider. |
`...triggerCharacters` | string[] | Trigger signature help when the user types one of the characters, like `,` or `(`. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

▸ **registerSignatureHelpProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [SignatureHelpProvider](../interfaces/_index_d_._plugin_.signaturehelpprovider.md), `metadata`: [SignatureHelpProviderMetadata](../interfaces/_index_d_._plugin_.signaturehelpprovidermetadata.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11149](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11149)*

#### Parameters:

Name | Type |
------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) |
`provider` | [SignatureHelpProvider](../interfaces/_index_d_._plugin_.signaturehelpprovider.md) |
`metadata` | [SignatureHelpProviderMetadata](../interfaces/_index_d_._plugin_.signaturehelpprovidermetadata.md) |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

___

### registerTypeDefinitionProvider

▸ **registerTypeDefinitionProvider**(`selector`: [DocumentSelector](_index_d_._plugin_.md#documentselector), `provider`: [TypeDefinitionProvider](../interfaces/_index_d_._plugin_.typedefinitionprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:10953](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10953)*

Register a type definition provider.

Multiple providers can be registered for a language. In that case providers are asked in
parallel and the results are merged. A failing provider (rejected promise or exception) will
not cause a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`selector` | [DocumentSelector](_index_d_._plugin_.md#documentselector) | A selector that defines the documents this provider is applicable to. |
`provider` | [TypeDefinitionProvider](../interfaces/_index_d_._plugin_.typedefinitionprovider.md) | A type definition provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### registerWorkspaceSymbolProvider

▸ **registerWorkspaceSymbolProvider**(`provider`: [WorkspaceSymbolProvider](../interfaces/_index_d_._plugin_.workspacesymbolprovider.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11030](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11030)*

Register a workspace symbol provider.

Multiple providers can be registered. In that case providers are asked in parallel and
the results are merged. A failing provider (rejected promise or exception) will not cause
a failure of the whole operation.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`provider` | [WorkspaceSymbolProvider](../interfaces/_index_d_._plugin_.workspacesymbolprovider.md) | A workspace symbol provider. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unregisters this provider when being disposed.

___

### setLanguageConfiguration

▸ **setLanguageConfiguration**(`language`: string, `configuration`: [LanguageConfiguration](../interfaces/_index_d_._plugin_.languageconfiguration.md)): [Disposable](../classes/_index_d_._plugin_.disposable.md)

*Defined in [index.d.ts:11236](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L11236)*

Set a [language configuration](#LanguageConfiguration) for a language.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`language` | string | A language identifier like `typescript`. |
`configuration` | [LanguageConfiguration](../interfaces/_index_d_._plugin_.languageconfiguration.md) | Language configuration. |

**Returns:** [Disposable](../classes/_index_d_._plugin_.disposable.md)

A [disposable](#Disposable) that unsets this configuration.

___

### setTextDocumentLanguage

▸ **setTextDocumentLanguage**(`document`: [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md), `languageId`: string): [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

*Defined in [index.d.ts:10798](https://github.com/shuyaqian/cloudide-plugin-api/blob/9d985be/index.d.ts#L10798)*

Set (and change) the [language](#TextDocument.languageId) that is associated
with the given document.

*Note* that calling this function will trigger the [`onDidCloseTextDocument`](#workspace.onDidCloseTextDocument) event
followed by the [`onDidOpenTextDocument`](#workspace.onDidOpenTextDocument) event.

#### Parameters:

Name | Type | Description |
------ | ------ | ------ |
`document` | [TextDocument](../interfaces/_index_d_._plugin_.textdocument.md) | The document which language is to be changed |
`languageId` | string | The new language identifier. |

**Returns:** [Thenable](../interfaces/_index_d_.thenable.md)\<[TextDocument](../interfaces/_index_d_._plugin_.textdocument.md)>

A thenable that resolves with the updated document.
