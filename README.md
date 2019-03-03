
# VS Code TYPO3 Flux Snippets

Visual Studio Code Snippet extension for TYPO3 Flux.

**Current status**

* 52 Snippets
* 1 Template

## Snippets overview

Not all arguments are included in a snippet, only the one which are (in my oppinion) mostyl used.<br>
*Snippets marked with a * are not used by myself so I dont know which arguments are mostly necessary.*

### \<flux:*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:form</td>
      <td>

```html
<flux:form id="$1" label="$2" description="$3" />
```
  </td>
  </tr>
    <tr>
      <td>flux:grid</td>
      <td>

```html
<flux:grid />
```
  </td>
  </tr>
    <tr>
      <td>flux:outlet</td>
      <td>

```html
<flux:outlet${1: enabled="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:variable</td>
      <td>

```html
<flux:variable name="$1" />
```
  </td>
  </tr>
  </tbody>
</table>

### \<flux:content.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:content.get</td>
      <td>

```html
<flux:content.get area="$1"${3: limit="$2"}${5: offset="$4"}${7: order="'${6:sorting}'"}${9: sortDirection="'${8:ASC}'"}${11: as="$10"}${13: loadRegister="$12"}${15: render="${14:1}"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:content.render</td>
      <td>

```html
<flux:content.render area="$1"${3: limit="$2"}${5: offset="$4"}${7: order="'${6:sorting}'"}${9: sortDirection="'${8:ASC}'"}${11: as="$10"}${13: loadRegister="$12"}${15: render="${14:1}"} />
```
  </td>
  </tr>
  </tbody>
</table>

### \<flux:field.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:field.inline.fal</td>
      <td>

```html
<flux:field.inline.fal name="$1" label="$2"${3: required="1"}${4: multiple="0"}${6: minItems="$5"}${8: maxItems="$7"}${9: collapseAll="0"}${10: expandSingle="0"} allowedExtensions="${11:jpg,jpeg,png,svg}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.tree.category*</td>
      <td>

```html
<flux:field.tree.category name="$1" label="$2"${3: required="1"}${4: multiple="0"}${6: minItems="$5"}${8: maxItems="$7"}${9: showThumbs="1"}${10: expandAll="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.checkbox</td>
      <td>

```html
<flux:field.checkbox name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${7: clear="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.controllerActions*</td>
      <td>

```html
<flux:field.controllerActions name="$1" label="$2" required="1" exclude="1"  extensionName="NULL" controllerExtensionName="NULL" pluginName="NULL" controllerName="NULL" actions="{foo: 'bar'}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.custom*</td>
      <td>

```html
<flux:field.custom name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${7: clear="1"}${9: userFunc="${8:FluidTYPO3\\Flux\\UserFunction\\HtmlOutput->renderField}"} />
  ```
  </td>
  </tr>
    <tr>
      <td>flux:field.file</td>
      <td>

```html
<flux:field.file name="$1" label="$2"${4: required="1"}${5: multiple="1"}${7: minItems="$6"}${9: maxItems="$8"}${11: allowed="${10:jpg,png,gif,svg}"}${12: showThumbnails="1"}${13: useFalRelation="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.inline*</td>
      <td>

```html
<flux:field.inline name="$1" label="$2" eextensionName="NULL" table="NULL" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.input</td>
      <td>

```html
<flux:field.input name="$1" label="$2"${4: default="$3"}${5: required="1"}${7: eval="${6:'trim'}"}${9: maxCharacters="$8"}${11: placeholder="$10"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.multiRelation*</td>
      <td>

```html
<flux:field.multiRelation name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.none</td>
      <td>

```html
<flux:field.none name="$1" label="$2" default="$3" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.radio</td>
      <td>

```html
<flux:field.radio name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"} items="{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.relation*</td>
      <td>

```html
<flux:field.relation name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.select</td>
      <td>

```html
<flux:field.select name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${12: renderType="${7:selectSingle}${8:selectSingleBox}${9:selectCheckBox}${10:selectMultipleSideBySide}${11:selectTree}"}${14: size="$13"}${16: maxItems="$15"} items="{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.text</td>
      <td>

```html
<flux:field.text name="$1" label="$2"${4: required="1"}${6: validate="'${5:trim}'"}${7: enableRichText="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.tree*</td>
      <td>

```html
<flux:field.tree name="$1" label="$2"${4: required="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:field.userFunc*</td>
      <td>

```html
<flux:field.userFunc name="$1" label="$2"${5: extensionName="$4"} userFunc="$6" />
```
  </td>
  </tr>
  </tbody>
</table>


### \<flux:form.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:form.option.group</td>
      <td>

```html
<flux:form.option.group value="$1" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.option.icon</td>
      <td>

```html
<flux:form.option.icon value="/typo3conf/ext/$1/Resources/Public/Icons/${2:icon.svg}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.option.sorting</td>
      <td>

```html
<flux:form.option.sorting value="$1" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.option.static</td>
      <td>

```html
<flux:form.option.static value="${1:1}" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.container</td>
      <td>

```html
<flux:form.container name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.content</td>
      <td>

```html
<flux:form.content name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.data</td>
      <td>

```html
<flux:form.data table="$1" field="$2" uid="$3" record="${4:{foo: 'bar'}}" as="$5" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.object</td>
      <td>

```html
<flux:form.object name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.option</td>
      <td>

```html
<flux:form.option name="$1" value="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.render</td>
      <td>

```html
<flux:form.render form="$1" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.section</td>
      <td>

```html
<flux:form.section name="$1" label="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.sheet</td>
      <td>

```html
<flux:form.sheet name="$1" label="$2"${4: description="$3"}${6: shortDescription="$5"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:form.variable</td>
      <td>

```html
<flux:form.variable name="$1" value="$2" />
```
  </td>
  </tr>
  </tbody>
</table>


### \<flux:grid.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:grid.column</td>
      <td>

```html
<flux:grid.column name="$1" label="$2" colPos="$3"${5: colspan="$4"}${7: rowspan="$6"}${9: style="$8"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:grid.row</td>
      <td>

```html
<flux:grid.row name="$1" label="$2" />
```
  </td>
  </tr>
  </tbody>
</table>

### \<flux:outlet.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:outlet.argument</td>
      <td>

```html
<flux:outlet.argument name="$1" type="$2" />
```
  </td>
  </tr>
    <tr>
      <td>flux:outlet.form</td>
      <td>

```html
<flux:outlet.form name="$1" action="$2" controller="$3" extensionName="$4" pluginName="$5" pageUid="$6" />
```
  </td>
  </tr>
    <tr>
      <td>flux:outlet.validate</td>
      <td>

```html
<flux:outlet.validate type="$1"${3: options="$2"} />
```
  </td>
  </tr>
  </tbody>
</table>

### \<flux:pipe.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:pipe.controller</td>
      <td>

```html
<flux:pipe.controller direction="$1" action="$2" controller="$3" extensionName="$4" />
```
  </td>
  </tr>
    <tr>
      <td>flux:pipe.email</td>
      <td>

```html
<flux:pipe.email direction="$1" body="$2" bodySection="$3" subject="$4" recipient="$5" sender="$6" />
```
  </td>
  </tr>
    <tr>
      <td>flux:pipe.flashMessage</td>
      <td>

```html
<flux:pipe.flashMessage direction="$1" message="$2" title="'$3'" severity="$4"${5: storeInSession="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:pipe.typeConverter</td>
      <td>

```html
<flux:pipe.typeConverter direction="$1" targetType="$2" typeConverter="$3" />
```
  </td>
  </tr>
  </tbody>
</table>

### \<flux:wizard.*\>

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>flux:wizard.add</td>
      <td>

```html
<flux:wizard.add label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pid="$6" setValue="'prepend'" />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.colorPicker</td>
      <td>

```html
<flux:wizard.colorPicker label="$1" dim="'${2:20x20}'" width="$3" height="$4" exampleImg="'${5:EXT:flux/Resources/Public/Icons/ColorWheel.png}'" />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.edit</td>
      <td>

```html
<flux:wizard.edit label="$1"${2: hideParent="1"}${4: extensionName="$3"} width="$5" height="$6"${7: openOnlyIfSelected="1"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.link</td>
      <td>

```html
<flux:wizard.link label="$1"${2: hideParent="1"}${4: extensionName="$3"} activeTab="'${5:file}'" width="$6" height="$7"${9: allowedExtensions="$8"} />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.list</td>
      <td>

```html
<flux:wizard.list label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pid="$6" width="$7" height="$8" />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.select</td>
      <td>

```html
<flux:wizard.select label="$1"${2: hideParent="1"}${4: extensionName="$3"} mode="'${5:substitution}'" items="$6" />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.slider</td>
      <td>

```html
<flux:wizard.slider label="$1"${2: hideParent="1"}${4: extensionName="$3"} mode="'${5:substitution}'" steps="$6" width="$7" />
```
  </td>
  </tr>
    <tr>
      <td>flux:wizard.suggest</td>
      <td>

```html
<flux:wizard.suggest label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pidList="'$6'" pidDepth="$7" minimumCharacters="$8" maxPathTitleLength="$9"${10: searchWholePhrase="1"} searchCondition="'$11'"${13: cssClass="'$12'"}${15: receiverClass="'$14'"}${17: renderFunc="'$16'"} />
```
  </td>
  </tr>
  </tbody>
</table>

## Templates overview

#### Trigger: flux-ce-template

<table>
  <thead>
    <tr>
      <th>Trigger</th><th>TYPO3 Code</th>
    </tr>
  </thead>
  <tbody>
      <tr>
      <td>flux-ce-template</td>
      <td>

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
  </td>
  </tr>
  </tbody>
</table>

## Source

All snippets have been taken from [fluidtypo3.org](https://fluidtypo3.org/viewhelpers/flux/master.html) ViewHelper reference<br>

## Recomendations

Works perfectly together with other TYPO3 snippet extension<br>
https://github.com/MrSilaz/typo3snippets<br>
https://github.com/febLey/vscode-typo3-vhs-snippets

## License

[GNU General Public License (GPL), Version 2.0](http://www.gnu.org/licenses/gpl-2.0.html)
