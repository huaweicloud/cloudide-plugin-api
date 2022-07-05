[@codearts/plugin](../README.md) / ["@codearts/plugin"](_codearts_plugin_.md) / languages

# Namespace: languages

["@codearts/plugin"](_codearts_plugin_.md).languages

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

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `name?` | `string` |  |

#### Returns

[`DiagnosticCollection`](../interfaces/codearts_plugin_.DiagnosticCollection.md)

#### Defined in

[index.d.ts:12323](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12323)

___

### createLanguageStatusItem

▸ **createLanguageStatusItem**(`id`, `selector`): [`LanguageStatusItem`](../interfaces/codearts_plugin_.LanguageStatusItem.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` |  |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |

#### Returns

[`LanguageStatusItem`](../interfaces/codearts_plugin_.LanguageStatusItem.md)

#### Defined in

[index.d.ts:12331](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12331)

___

### getDiagnostics

▸ **getDiagnostics**(`resource`): [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `resource` | [`Uri`](../classes/codearts_plugin_.Uri.md) |  |

#### Returns

[`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]

#### Defined in

[index.d.ts:12308](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12308)

▸ **getDiagnostics**(): [[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

#### Returns

[[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

#### Defined in

[index.d.ts:12315](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12315)

___

### getLanguages

▸ **getLanguages**(): [`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Defined in

[index.d.ts:12234](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12234)

___

### match

▸ **match**(`selector`, `document`): `number`

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) |  |

#### Returns

`number`

#### Defined in

[index.d.ts:12294](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12294)

___

### onDidChangeDiagnostics

▸ `Const` **onDidChangeDiagnostics**(`listener`, `thisArgs?`, `disposables?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `listener` | (`e`: [`DiagnosticChangeEvent`](../interfaces/codearts_plugin_.DiagnosticChangeEvent.md)) => `any` |
| `thisArgs?` | `any` |
| `disposables?` | [`Disposable`](../classes/codearts_plugin_.Disposable.md)[] |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12300](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12300)

___

### registerCallHierarchyProvider

▸ **registerCallHierarchyProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`CallHierarchyProvider`](../interfaces/codearts_plugin_.CallHierarchyProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12720](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12720)

___

### registerCodeActionsProvider

▸ **registerCodeActionsProvider**(`selector`, `provider`, `metadata?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`CodeActionProvider`](../interfaces/codearts_plugin_.CodeActionProvider.md)<[`CodeAction`](../classes/codearts_plugin_.CodeAction.md)\> |  |
| `metadata?` | [`CodeActionProviderMetadata`](../interfaces/codearts_plugin_.CodeActionProviderMetadata.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12379](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12379)

___

### registerCodeLensProvider

▸ **registerCodeLensProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`CodeLensProvider`](../interfaces/codearts_plugin_.CodeLensProvider.md)<[`CodeLens`](../classes/codearts_plugin_.CodeLens.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12392](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12392)

___

### registerColorProvider

▸ **registerColorProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentColorProvider`](../interfaces/codearts_plugin_.DocumentColorProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12668](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12668)

___

### registerCompletionItemProvider

▸ **registerCompletionItemProvider**(`selector`, `provider`, ...`triggerCharacters`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`CompletionItemProvider`](../interfaces/codearts_plugin_.CompletionItemProvider.md)<[`CompletionItem`](../classes/codearts_plugin_.CompletionItem.md)\> |  |
| `...triggerCharacters` | `string`[] |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12352](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12352)

___

### registerDeclarationProvider

▸ **registerDeclarationProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DeclarationProvider`](../interfaces/codearts_plugin_.DeclarationProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12444](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12444)

___

### registerDefinitionProvider

▸ **registerDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DefinitionProvider`](../interfaces/codearts_plugin_.DefinitionProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12405](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12405)

___

### registerDocumentFormattingEditProvider

▸ **registerDocumentFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentFormattingEditProvider`](../interfaces/codearts_plugin_.DocumentFormattingEditProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12594](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12594)

___

### registerDocumentHighlightProvider

▸ **registerDocumentHighlightProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentHighlightProvider`](../interfaces/codearts_plugin_.DocumentHighlightProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12497](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12497)

___

### registerDocumentLinkProvider

▸ **registerDocumentLinkProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentLinkProvider`](../interfaces/codearts_plugin_.DocumentLinkProvider.md)<[`DocumentLink`](../classes/codearts_plugin_.DocumentLink.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12655](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12655)

___

### registerDocumentRangeFormattingEditProvider

▸ **registerDocumentRangeFormattingEditProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentRangeFormattingEditProvider`](../interfaces/codearts_plugin_.DocumentRangeFormattingEditProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12611](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12611)

___

### registerDocumentRangeSemanticTokensProvider

▸ **registerDocumentRangeSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentRangeSemanticTokensProvider`](../interfaces/codearts_plugin_.DocumentRangeSemanticTokensProvider.md) |  |
| `legend` | [`SemanticTokensLegend`](../classes/codearts_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12581](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12581)

___

### registerDocumentSemanticTokensProvider

▸ **registerDocumentSemanticTokensProvider**(`selector`, `provider`, `legend`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentSemanticTokensProvider`](../interfaces/codearts_plugin_.DocumentSemanticTokensProvider.md) |  |
| `legend` | [`SemanticTokensLegend`](../classes/codearts_plugin_.SemanticTokensLegend.md) | - |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12562](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12562)

___

### registerDocumentSymbolProvider

▸ **registerDocumentSymbolProvider**(`selector`, `provider`, `metaData?`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`DocumentSymbolProvider`](../interfaces/codearts_plugin_.DocumentSymbolProvider.md) |  |
| `metaData?` | [`DocumentSymbolProviderMetadata`](../interfaces/codearts_plugin_.DocumentSymbolProviderMetadata.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12511](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12511)

___

### registerEvaluatableExpressionProvider

▸ **registerEvaluatableExpressionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`EvaluatableExpressionProvider`](../interfaces/codearts_plugin_.EvaluatableExpressionProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12469](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12469)

___

### registerFoldingRangeProvider

▸ **registerFoldingRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`FoldingRangeProvider`](../interfaces/codearts_plugin_.FoldingRangeProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12698](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12698)

___

### registerHoverProvider

▸ **registerHoverProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`HoverProvider`](../interfaces/codearts_plugin_.HoverProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12457](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12457)

___

### registerImplementationProvider

▸ **registerImplementationProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`ImplementationProvider`](../interfaces/codearts_plugin_.ImplementationProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12418](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12418)

___

### registerInlayHintsProvider

▸ **registerInlayHintsProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`InlayHintsProvider`](../interfaces/codearts_plugin_.InlayHintsProvider.md)<[`InlayHint`](../classes/codearts_plugin_.InlayHint.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12681](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12681)

___

### registerInlineCompletionItemProvider

▸ **registerInlineCompletionItemProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`InlineCompletionItemProvider`](../interfaces/codearts_plugin_.InlineCompletionItemProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12365](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12365)

___

### registerInlineValuesProvider

▸ **registerInlineValuesProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`InlineValuesProvider`](../interfaces/codearts_plugin_.InlineValuesProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12484](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12484)

___

### registerLinkedEditingRangeProvider

▸ **registerLinkedEditingRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`LinkedEditingRangeProvider`](../interfaces/codearts_plugin_.LinkedEditingRangeProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12742](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12742)

___

### registerOnTypeFormattingEditProvider

▸ **registerOnTypeFormattingEditProvider**(`selector`, `provider`, `firstTriggerCharacter`, ...`moreTriggerCharacter`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`OnTypeFormattingEditProvider`](../interfaces/codearts_plugin_.OnTypeFormattingEditProvider.md) |  |
| `firstTriggerCharacter` | `string` |  |
| `...moreTriggerCharacter` | `string`[] |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12626](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12626)

___

### registerReferenceProvider

▸ **registerReferenceProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`ReferenceProvider`](../interfaces/codearts_plugin_.ReferenceProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12536](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12536)

___

### registerRenameProvider

▸ **registerRenameProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`RenameProvider`](../interfaces/codearts_plugin_.RenameProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12549](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12549)

___

### registerSelectionRangeProvider

▸ **registerSelectionRangeProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`SelectionRangeProvider`](../interfaces/codearts_plugin_.SelectionRangeProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12711](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12711)

___

### registerSignatureHelpProvider

▸ **registerSignatureHelpProvider**(`selector`, `provider`, ...`triggerCharacters`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`SignatureHelpProvider`](../interfaces/codearts_plugin_.SignatureHelpProvider.md) |  |
| `...triggerCharacters` | `string`[] |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12641](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12641)

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

[index.d.ts:12642](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12642)

___

### registerTypeDefinitionProvider

▸ **registerTypeDefinitionProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`TypeDefinitionProvider`](../interfaces/codearts_plugin_.TypeDefinitionProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12431](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12431)

___

### registerTypeHierarchyProvider

▸ **registerTypeHierarchyProvider**(`selector`, `provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `selector` | [`DocumentSelector`](_codearts_plugin_.md#documentselector) |  |
| `provider` | [`TypeHierarchyProvider`](../interfaces/codearts_plugin_.TypeHierarchyProvider.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12729](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12729)

___

### registerWorkspaceSymbolProvider

▸ **registerWorkspaceSymbolProvider**(`provider`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `provider` | [`WorkspaceSymbolProvider`](../interfaces/codearts_plugin_.WorkspaceSymbolProvider.md)<[`SymbolInformation`](../classes/codearts_plugin_.SymbolInformation.md)\> |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12523](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12523)

___

### setLanguageConfiguration

▸ **setLanguageConfiguration**(`language`, `configuration`): [`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `language` | `string` |  |
| `configuration` | [`LanguageConfiguration`](../interfaces/codearts_plugin_.LanguageConfiguration.md) |  |

#### Returns

[`Disposable`](../classes/codearts_plugin_.Disposable.md)

#### Defined in

[index.d.ts:12751](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12751)

___

### setTextDocumentLanguage

▸ **setTextDocumentLanguage**(`document`, `languageId`): [`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `document` | [`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md) |  |
| `languageId` | `string` |  |

#### Returns

[`Thenable`](../interfaces/Thenable.md)<[`TextDocument`](../interfaces/codearts_plugin_.TextDocument.md)\>

#### Defined in

[index.d.ts:12247](https://github.com/huaweicloud/cloudide-plugin-api/blob/d4de966/index.d.ts#L12247)
