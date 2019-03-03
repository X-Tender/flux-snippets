
# VS Code TYPO3 Flux Snippets

Visual Studio Code Snippet extension for TYPO3 Flux.

**Current status**

* 52 Snippets
* 1 Template

## Snippets overview

Not all arguments are included in a snippet, only the one which are (in my oppinion) mostyl used.<br>
*Snippets marked with a * are not used by myself so I dont know which arguments are mostly necessary.*

### \<flux:*\>

Trigger | TYPO3 Code
--- | ---
flux:form | <code><flux:form id=\"$1\" label=\"$2\" description=\"$3\" /></code>
flux:grid | <code>\<flux:grid /></code>
flux:outlet | <code>\<flux:outlet${2: enabled=\"${1:1}\"} /></code>
flux:variable | <code>\<flux:variable name=\"$1\" /></code>

### \<flux:content.*\>

Trigger | TYPO3 Code
--- | ---
flux:content.get | <code>\<flux:content.get area=\"$1\"${3: limit=\"$2\"}${5: offset=\"$4\"}${7: order=\"'${6:sorting}'\"}${9: sortDirection=\"'${8:ASC}'\"}${11: as=\"$10\"}${13: loadRegister=\"$12\"}${15: render=\"${14:1}\"} /></code>
flux:content.render | <code>\<flux:content.render area=\"$1\"${3: limit=\"$2\"}${5: offset=\"$4\"}${7: order=\"'${6:sorting}'\"}${9: sortDirection=\"'${8:ASC}'\"}${11: as=\"$10\"}${13: loadRegister=\"$12\"}${15: render=\"${14:1}\"} /></code>

### \<flux:field.*\>

Trigger | TYPO3 Code
--- | ---
flux:field.inline.fal | <code>\<flux:field.inline.fal name=\"$1\" label=\"$2\"${3: required=\"1\"}${4: multiple=\"0\"}${6: minItems=\"$5\"}${8: maxItems=\"$7\"}${9: collapseAll=\"0\"}${10: expandSingle=\"0\"} allowedExtensions=\"${11:jpg,jpeg,png,svg}\" /></code>
flux:field.tree.category* | <code>\<flux:field.tree.category name=\"$1\" label=\"$2\"${3: required=\"1\"}${4: multiple=\"0\"}${6: minItems=\"$5\"}${8: maxItems=\"$7\"}${9: showThumbs=\"1\"}${10: expandAll=\"1\"} /></code>
flux:field.checkbox | <code>\<flux:field.checkbox name=\"$1\" label=\"$2\"${4: default=\"$3\"}${5: required=\"1\"}${6: requestUpdate=\"1\"}${7: clear=\"1\"} /></code>
flux:field.controllerActions* | <code>\<flux:field.controllerActions name=\"$1\" label=\"$2\" required=\"1\" exclude=\"1\"  extensionName=\"NULL\" controllerExtensionName=\"NULL\" pluginName=\"NULL\" controllerName=\"NULL\" actions=\"{foo: 'bar'}\" /></code>
flux:field.custom* | <code>\<flux:field.custom name=\"$1\" label=\"$2\"${4: default=\"$3\"}${5: required=\"1\"}${6: requestUpdate=\"1\"}${7: clear=\"1\"}${9: userFunc=\"${8:FluidTYPO3\\Flux\\UserFunction\\HtmlOutput->renderField}\"} /></code>
flux:field.file | <code>\<flux:field.file name=\"$1\" label=\"$2\"${4: required=\"1\"}${5: multiple=\"1\"}${7: minItems=\"$6\"}${9: maxItems=\"$8\"}${11: allowed=\"${10:jpg,png,gif,svg}\"}${12: showThumbnails=\"1\"}${13: useFalRelation=\"1\"} /></code>
flux:field.inline* | <code>\<flux:field.inline name=\"$1\" label=\"$2\" eextensionName=\"NULL\" table=\"NULL\" /></code>
flux:field.input | <code>\<flux:field.input name=\"$1\" label=\"$2\"${4: default=\"$3\"}${5: required=\"1\"}${7: eval=\"${6:'trim'}\"}${9: maxCharacters=\"$8\"}${11: placeholder=\"$10\"} /></code>
flux:field.multiRelation* | <code>\<flux:field.multiRelation name=\"$1\" label=\"$2\" /></code>
flux:field.none | <code>\<flux:field.none name=\"$1\" label=\"$2\" default=\"$3\" /></code>
flux:field.radio | <code>\<flux:field.radio name=\"$1\" label=\"$2\"${4: default=\"$3\"}${5: required=\"1\"}${6: requestUpdate=\"1\"} items=\"{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}\" /></code>
flux:field.relation* | <code>\<flux:field.relation name=\"$1\" label=\"$2\" /></code>
flux:field.select | <code>\<flux:field.select name=\"$1\" label=\"$2\"${4: default=\"$3\"}${5: required=\"1\"}${6: requestUpdate=\"1\"}${12: renderType=\"${7:selectSingle}${8:selectSingleBox}${9:selectCheckBox}${10:selectMultipleSideBySide}${11:selectTree}\"}${14: size=\"$13\"}${16: maxItems=\"$15\"} items=\"{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}\" /></code>
flux:field.text | <code>\<flux:field.text name=\"$1\" label=\"$2\"${4: required=\"1\"}${6: validate=\"'${5:trim}'\"}${7: enableRichText=\"1\"} /></code>
flux:field.tree* | <code>\<flux:field.tree name=\"$1\" label=\"$2\"${4: required=\"1\"} /></code>
flux:field.userFunc* | <code>\<flux:field.userFunc name=\"$1\" label=\"$2\"${5: extensionName=\"$4\"} userFunc=\"$6\" /></code>

### \<flux:form.*\>

Trigger | TYPO3 Code
--- | ---
flux:form.option.group | <code>\<flux:form.option.group value=\"$1\" /></code>
flux:form.option.icon | <code>\<flux:form.option.icon value=\"/typo3conf/ext/$1/Resources/Public/Icons/${2:icon.svg}\" /></code>
flux:form.option.sorting | <code>\<flux:form.option.sorting value=\"$1\" /></code>
flux:form.option.static | <code>\<flux:form.option.static value=\"${1:1}\" /></code>
flux:form.container | <code>\<flux:form.container name=\"$1\" label=\"$2\" /></code>
flux:form.content | <code>\<flux:form.content name=\"$1\" label=\"$2\" /></code>
flux:form.data | <code>\<flux:form.data table=\"$1\" field=\"$2\" uid=\"$3\" record=\"${4:{foo: 'bar'}}\" as=\"$5\" /></code>
flux:form.object | <code>\<flux:form.object name=\"$1\" label=\"$2\" /></code>
flux:form.option | <code>\<flux:form.option name=\"$1\" value=\"$2\" /></code>
flux:form.render | <code>\<flux:form.render form=\"$1\" /></code>
flux:form.section | <code>\<flux:form.section name=\"$1\" label=\"$2\" /></code>
flux:form.sheet | <code>\<flux:form.sheet name=\"$1\" label=\"$2\"${4: description=\"$3\"}${6: shortDescription=\"$5\"} /></code>
flux:form.variable | <code>\<flux:form.variable name=\"$1\" value=\"$2\" /></code>

### \<flux:grid.*\>

Trigger | TYPO3 Code
--- | ---
flux:grid.column | <code>\<flux:grid.column name=\"$1\" label=\"$2\" colPos=\"$3\"${5: colspan=\"$4\"}${7: rowspan=\"$6\"}${9: style=\"$8\"} /></code>
flux:grid.row | <code>\<flux:grid.row name=\"$1\" label=\"$2\" /></code>

### \<flux:outlet.*\>

Trigger | TYPO3 Code
--- | ---
flux:outlet.argument | <code>\<flux:outlet.argument name=\"$1\" type=\"$2\" /></code>
flux:outlet.form | <code>\<flux:outlet.form name=\"$1\" action=\"$2\" controller=\"$3\" extensionName=\"$4\" pluginName=\"$5\" pageUid=\"$6\" /></code>
flux:outlet.validate | <code>\<flux:outlet.validate type=\"$1\"${3: options=\"$2\"} /></code>

### \<flux:pipe.*\>

Trigger | TYPO3 Code
--- | ---
flux:pipe.controller | <code>\<flux:pipe.controller direction=\"$1\" action=\"$2\" controller=\"$3\" extensionName=\"$4\" /></code>
flux:pipe.email | <code>\<flux:pipe.email direction=\"$1\" body=\"$2\" bodySection=\"$3\" subject=\"$4\" recipient=\"$5\" sender=\"$6\" /></code>
flux:pipe.flashMessage | <code>\<flux:pipe.flashMessage direction=\"$1\" message=\"$2\" title=\"'$3'\" severity=\"$4\"${5: storeInSession=\"1\"} /></code>
flux:pipe.typeConverter | <code>\<flux:pipe.typeConverter direction=\"$1\" targetType=\"$2\" typeConverter=\"$3\" /></code>

### \<flux:wizard.*\>

Trigger | TYPO3 Code
--- | ---
flux:wizard.add | <code>\<flux:wizard.add label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} table=\"$5\" pid=\"$6\" setValue=\"'prepend'\" /></code>
flux:wizard.colorPicker | <code>\<flux:wizard.colorPicker label=\"$1\" dim=\"'${2:20x20}'\" width=\"$3\" height=\"$4\" exampleImg=\"'${5:EXT:flux/Resources/Public/Icons/ColorWheel.png}'\" /></code>
flux:wizard.edit | <code>\<flux:wizard.edit label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} width=\"$5\" height=\"$6\"${7: openOnlyIfSelected=\"1\"} /></code>
flux:wizard.link | <code>\<flux:wizard.link label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} activeTab=\"'${5:file}'\" width=\"$6\" height=\"$7\"${9: allowedExtensions=\"$8\"} /></code>
flux:wizard.list | <code>\<flux:wizard.list label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} table=\"$5\" pid=\"$6\" width=\"$7\" height=\"$8\" /></code>
flux:wizard.select | <code>\<flux:wizard.select label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} mode=\"'${5:substitution}'\" items=\"$6\" /></code>
flux:wizard.slider | <code>\<flux:wizard.slider label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} mode=\"'${5:substitution}'\" steps=\"$6\" width=\"$7\" /></code>
flux:wizard.suggest | <code>\<flux:wizard.suggest label=\"$1\"${2: hideParent=\"1\"}${4: extensionName=\"$3\"} table=\"$5\" pidList=\"'$6'\" pidDepth=\"$7\" minimumCharacters=\"$8\" maxPathTitleLength=\"$9\"${10: searchWholePhrase=\"1\"} searchCondition=\"'$11'\"${13: cssClass=\"'$12'\"}${15: receiverClass=\"'$14'\"}${17: renderFunc=\"'$16'\"} /></code>

## Templates overview

#### Trigger: flux-ce-template
```html
<div xmlns="http://www.w3.org/1999/xhtml" lang="en"
  xmlns:f="http://typo3.org/ns/TYPO3/Fluid/ViewHelpers"
  xmlns:flux="http://typo3.org/ns/FluidTYPO3/Flux/ViewHelpers"
  xmlns:v="http://typo3.org/ns/FluidTYPO3/Vhs/ViewHelpers">

  <f:layout name="Content" />

  <f:section name="Configuration">
    <flux:form
      id="$1"
      label="$2"
      description="$3"
    >
      <flux:form.option name="group" value="$4" />
      <flux:form.option name="icon" value="EXT:$5/Resources/Public/Icons/Content/icon.svg" />
      $6
    </flux:form>
  </f:section>

  <f:section name="Preview">
    $7
  </f:section>

  <f:section name="Main">
    $8
  </f:section>
</div>
```

## Source

All snippets have been taken from [fluidtypo3.org](https://fluidtypo3.org/viewhelpers/flux/master.html) ViewHelper reference<br>

## Recomendations

Works perfectly together with other TYPO3 snippet extension<br>
https://github.com/MrSilaz/typo3snippets<br>
https://github.com/febLey/vscode-typo3-vhs-snippets

## License

[GNU General Public License (GPL), Version 2.0](http://www.gnu.org/licenses/gpl-2.0.html)
