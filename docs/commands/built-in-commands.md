# Build-in Commands

List of common built-in commands in theia.

## 1. Common Commands
### core.open
### core.copy
### core.paste
### core.copy.path
#### Parameters:
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |
### core.undo
### core.redo
### core.selectAll
### core.nextTab
### core.previousTab
### core.nextTabInGroup
### core.previousTabInGroup
### core.nextTabGroup
### core.previousTabBar
### core.close.tab
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.close.other.tabs
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.close.right.tabs
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.close.all.tabs
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.close.main.tab
### core.close.other.main.tabs
### core.close.all.main.tabs
### core.collapse.tab
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.collapse.all.tabs
### core.toggle.bottom.panel
### core.toggleMaximized
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### core.save
### core.saveWithoutFormatting
### core.saveAll
### core.about
### core.openView
### workbench.action.selectTheme
### workbench.action.selectIconTheme


## 2. Workspace Commands
### workspace:open
### workspace:openFile
### workspace:openFolder
### workspace:openWorkspace
### workspace:close
### workspace:openRecent
### workspace:saveAs
### file.saveAs
Name | Type |
------ | ------ |
`uri` | [URI](classes/_index_d_._plugin_.uri.md) |
### file.newFile
Name | Type |
------ | ------ |
`uri` | [URI](classes/_index_d_._plugin_.uri.md) |
### file.newFolder
Name | Type |
------ | ------ |
`uri` | [URI](classes/_index_d_._plugin_.uri.md) |
### file.rename
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |
### file.duplicate
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |
### file.delete
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |
### file.compare
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |
### workspace:addFolder
### workspace:removeFolder
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |

## 3. Git Commands
### git.clone
Name | Type |
------ | ------ |
`url?` | string |
`folder?` | string |
`branch?` | string |
### git.fetch
### git.pull.default
### git.pull
### git.push.default
### git.push
### git.merge
### git.checkout
### git.commit.all
### git-commit-add-sign-off
### git.commit.amend
### git.commit.signOff
### git.open.file
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### git.open.changes
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### git.sync
### git.publish
### git.stage.all
### git.unstage.all
### git.discard.all
### git.stash
### git.stash.apply
### git.stash.apply.latest
### git.commit.stash.pop
### git.commit.stash.drop
### git-refresh
### git-init

## 4. Git-Diff Commands
### git-diff:open-file-diff
Name | Type |
------ | ------ |
`fileUri` | [URI](classes/_index_d_._plugin_.uri.md) |
### git.navigate-changes.previous
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### git.navigate-changes.next
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |

## 5. Terminal Commands
### terminal:new
### terminal:<zero-width space>new:active:workspace
### terminal:clear
### terminal:context
Name | Type |
------ | ------ |
`uri` | [URI](classes/_index_d_._plugin_.uri.md) |
### terminal:split
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### terminal:find
### terminal:find:cancel
### terminal:<zero-width space>scroll:line:up
### terminal:<zero-width space>scroll:line:down
### terminal:<zero-width space>scroll:top
### terminal:<zero-width space>scroll:page:up
### terminal:<zero-width space>scroll:page:down

## 6. Output Commands
### output:append
Name | Type |
------ | ------ |
`name` | string |
`text` | string |
### output:appendLine
Name | Type |
------ | ------ |
`name` | string |
`text` | string |
### output:clear
Name | Type |
------ | ------ |
`name` | string |
### output:show
Name | Type |
------ | ------ |
`name` | string |
`options` | { preserveFocus?: boolean } |
### output:hide
Name | Type |
------ | ------ |
`name` | string |
### output:dispose
Name | Type |
------ | ------ |
`name` | string |
### output:widget:clear
### output:widget:lock
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### output:widget:unlock
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### output:pick-clear
### output:pick-show
### output:pick-hide
### output:pick-dispose
### output:copy-all


## 7. Vscode Commands
### vscode.openFolder
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`arg` | boolean &#124; IOpenFolderAPICommandOptions |
```
interface IOpenFolderAPICommandOptions {
    forceNewWindow?: boolean;
    forceReuseWindow?: boolean;
    noRecentEntry?: boolean;
}
```
### workbench.action.files.newUntitledFile
### workbench.action.files.openFile
### workbench.action.files.openFolder
### workbench.action.addRootFolder
### workbench.action.gotoLine
### workbench.action.quickOpen
### workbench.action.openSettings
### workbench.extensions.installExtension
Name | Type |
------ | ------ |
`vsixUriOrExtensionId` | UriComponents &#124; string |
```
interface UriComponents {
    scheme: string;
    authority: string;
    path: string;
    query: string;
    fragment: string;
    external?: string;
}
```
### workbench.action.files.save
Name | Type |
------ | ------ |
`uri?` | [monaco.Uri](https://microsoft.github.io/monaco-editor/api/classes/monaco.uri.html) |
### workbench.action.files.saveAll
### workbench.action.closeActiveEditor
Name | Type |
------ | ------ |
`uri?` | [monaco.Uri](https://microsoft.github.io/monaco-editor/api/classes/monaco.uri.html) |
### workbench.action.closeOtherEditors
Name | Type |
------ | ------ |
`uri?` | [monaco.Uri](https://microsoft.github.io/monaco-editor/api/classes/monaco.uri.html) |
### workbench.action.closeEditorsInGroup
Name | Type |
------ | ------ |
`uri?` | [monaco.Uri](https://microsoft.github.io/monaco-editor/api/classes/monaco.uri.html) |
### workbench.action.closeEditorsInOtherGroups
### workbench.action.closeEditorsToTheLeft
### workbench.action.closeEditorsToTheRight
### workbench.action.closeAllEditors
### workbench.action.nextEditor
### workbench.action.previousEditor
### workbench.action.navigateBack
### workbench.action.navigateForward
### workbench.action.navigateToLastEditLocation
### openInTerminal
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
### workbench.action.revertAndCloseActiveEditor
### vscode.executeDefinitionProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | Position |
#### Position
 ```
 interface Position {
    lineNumber: number;
    column: number;
}   
 ```
### vscode.executeDeclarationProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeTypeDefinitionProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeImplementationProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeHoverProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeDocumentHighlights
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeReferenceProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### vscode.executeDocumentSymbolProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
### vscode.executeFormatDocumentProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`options` | FormattingOptions |
#### FormattingOptions
```
 interface FormattingOptions {
    tabSize: number;
    insertSpaces: boolean;
}
```
### vscode.executeFormatOnTypeProvider
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
`ch` | string |
`options` | [FormattingOptions](#FormattingOptions) |
### vscode.prepareCallHierarchy
Name | Type |
------ | ------ |
`resource` | [URI](classes/_index_d_._plugin_.uri.md) |
`position` | [Position](#Position) |
### workbench.action.openRecent
### explorer.newFolder
### workbench.action.terminal.sendSequence
Name | Type |
------ | ------ |
`args?` | { text?: string } |
### workbench.action.terminal.kill
### workbench.view.explorer
### copyFilePath
### copyRelativeFilePath


## 8. Debug Commands
### workbench.action.debug.stop
### workbench.action.debug.restart
### debug.configurations.open
### debug.configurations.add
### workbench.action.debug.stepOver
### workbench.action.debug.stepInto
### workbench.action.debug.stepOut
### workbench.action.debug.continue
### workbench.action.debug.pause
### debug.thread.continue.all
### debug.thread.pause.all
### editor.debug.action.toggleBreakpoint
### editor.debug.action.inlineBreakpoint     
### debug.breakpoint.add.conditional
### debug.breakpoint.add.logpoint
### debug.breakpoint.add.function
### debug.breakpoint.disableAll
### debug.breakpoint.edit
### debug.logpoint.edit
### debug.breakpoint.remove
### debug.logpoint.remove
### debug.breakpoint.removeAll
### debug.breakpoint.toggleEnabled
### editor.debug.action.showDebugHover
### debug.frame.restart
### debug.callStack.copy
### debug.variable.setValue    
### debug.variable.copyValue
### debug.variable.copyAsExpression  
### debug.variable.watch   
### debug.watch.addExpression  
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### debug.watch.editExpression  
### debug.watch.copyExpressionValue 
### debug.watch.removeExpression   
### debug.watch.collapseAllExpressions  
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### debug.watch.removeAllExpressions
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### debug.thread.context.context.next
### debug.thread.context.stepin   
### debug.thread.context.stepout
### debug.thread.context.continue   
### debug.thread.context.pause  
### debug.thread.context.terminate   
### debug.session.context.stop  
### debug.session.context.restart   
### debug.session.context.pauseAll   
### debug.session.context.continueAll 
### debug.session.context.reveal    
### debug.session.context.openLeft
### debug.session.context.openRight   
### debug.session.context.openBottom   
### debug.editor.context.addBreakpoint
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.addBreakpoint.conditional
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.add.logpoint 
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.removeBreakpoint
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.edit.breakpoint
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.enableBreakpoint   
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.disableBreakpoint
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.logpoint.remove
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.logpoint.edit
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.logpoint.enable
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.editor.context.logpoint.disable
Name | Type |
------ | ------ |
`position` | [monaco.Position](https://microsoft.github.io/monaco-editor/api/classes/monaco.position.html) |
### debug.breakpointWidget.accept 
### debug.breakpointWidget.close 


## 9. Task Command
### task:run
### task:run:build  
### task:run:test
### workbench.action.tasks.runTask   
### task:run:last   
### task:attach
### task:run:text   
### task:configure  
### task:open_user
### task:clear-history  
### task:show-running   
### task:terminate
### task:restart-running  


## 10. Editor Command
### textEditor.commands.showReferences 
### textEditor.commands.configIndentation
### textEditor.commands.configEol   
### textEditor.commands.indentUsingSpaces  
### textEditor.commands.indentUsingTabs
### textEditor.change.language
### textEditor.change.encoding   
### textEditor.commands.go.back  
### textEditor.commands.go.forward   
### textEditor.commands.go.lastEdit  
### textEditor.commands.clear.history   
### workbench.action.showAllEditors  
### editor.action.toggleMinimap   
### editor.action.toggleRenderWhitespace
### editor.action.toggleWordWrap



## 11. Navigator Command
### navigator.reveal
Name | Type |
------ | ------ |
`event?` | [Event](https://github.com/microsoft/TypeScript/blob/master/lib/lib.dom.d.ts#L5346) |
### navigator.toggle.hidden.files
### navigator.toggle.autoReveal  
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### navigator.refresh 
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### navigator.collapse.all
Name | Type |
------ | ------ |
`widget` | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) |
### navigator.addRootFolder  
### workbench.files.action.focusFilesExplorer    
### navigator.copyRelativeFilePath
Name | Type |
------ | ------ |
`uris` | [URI[]](classes/_index_d_._plugin_.uri.md) |  
### navigator.open   
### compare:first    
### compare:second   


## 12. Perferences Command
### preferences:open
### preferences:copyJson.name
Name | Type |
------ | ------ |
{ id, value } | { id: string, value: string; } |  
### preferences:reset
Name | Type |
------ | ------ |
{ id } | { id: string } |  
### preferences:copyJson.value
Name | Type |
------ | ------ |
{ id, value } | { id: string, value: string; } |  



## 13. Search Command
### search-in-workspace.toggle
### search-in-workspace.open 
### search-in-workspace.in-folder
Name | Type |
------ | ------ |
uris | [URI[]](classes/_index_d_._plugin_.uri.md) |  
### search-in-workspace.refresh
Name | Type |
------ | ------ |
widget | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) | 
### search-in-workspace.cancel
Name | Type |
------ | ------ |
widget | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) | 
### search-in-workspace.collapse-all
Name | Type |
------ | ------ |
widget | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) | 
### search-in-workspace.clear-all 
Name | Type |
------ | ------ |
widget | [Widget](http://phosphorjs.github.io/phosphor/api/widgets/classes/widget.html) | 



## 14. Console Command
### console.selectAll 
### console.collapseAll
### console.clear
### console.execute  
### console.navigatePrevious
### console.navigateNext


## 15. Electron Menu Command
### theia.toggleDevTools
### view.reload  
### view.zoomIn  
### view.zoomOut  
### view.resetZoom   
### close.window  
