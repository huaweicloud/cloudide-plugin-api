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

[index.d.ts:12353](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12353)

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

[index.d.ts:12361](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12361)

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

[index.d.ts:12338](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12338)

▸ **getDiagnostics**(): [[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

#### Returns

[[`Uri`](../classes/codearts_plugin_.Uri.md), [`Diagnostic`](../classes/codearts_plugin_.Diagnostic.md)[]][]

#### Defined in

[index.d.ts:12345](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12345)

___

### getLanguages

▸ **getLanguages**(): [`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Returns

[`Thenable`](../interfaces/Thenable.md)<`string`[]\>

#### Defined in

[index.d.ts:12264](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12264)

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

[index.d.ts:12324](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12324)

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

[index.d.ts:12330](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12330)

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

[index.d.ts:12750](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12750)

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

[index.d.ts:12409](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12409)

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

[index.d.ts:12422](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12422)

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

[index.d.ts:12698](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12698)

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

[index.d.ts:12382](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12382)

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

[index.d.ts:12474](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12474)

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

[index.d.ts:12435](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12435)

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

[index.d.ts:12624](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12624)

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

[index.d.ts:12527](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12527)

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

[index.d.ts:12685](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12685)

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

[index.d.ts:12641](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12641)

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

[index.d.ts:12611](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12611)

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

[index.d.ts:12592](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12592)

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

[index.d.ts:12541](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12541)

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

[index.d.ts:12499](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12499)

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

[index.d.ts:12728](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12728)

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

[index.d.ts:12487](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12487)

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

[index.d.ts:12448](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12448)

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

[index.d.ts:12711](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12711)

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

[index.d.ts:12395](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12395)

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

[index.d.ts:12514](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12514)

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

[index.d.ts:12772](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12772)

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

[index.d.ts:12656](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12656)

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

[index.d.ts:12566](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12566)

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

[index.d.ts:12579](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12579)

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

[index.d.ts:12741](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12741)

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

[index.d.ts:12671](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12671)

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

[index.d.ts:12672](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12672)

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

[index.d.ts:12461](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12461)

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

[index.d.ts:12759](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12759)

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

[index.d.ts:12553](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12553)

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

[index.d.ts:12781](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12781)

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

[index.d.ts:12277](https://github.com/huaweicloud/cloudide-plugin-api/blob/3b0eee8/index.d.ts#L12277)
