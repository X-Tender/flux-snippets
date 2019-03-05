
# VS Code TYPO3 Flux Snippets

Visual Studio Code Snippet extension for TYPO3 Flux.

**Current status**

* 52 Snippets
* 1 Template

## Snippets overview

Not all arguments are included in a snippet, only the one which are (in my oppinion) mostyl used.<br>
*Snippets marked with a * are not used by myself so I dont know which arguments are mostly necessary.*

### \<flux:*\>

#### flux:form
```html
<flux:form id="$1" label="$2" description="$3" />
```

#### flux:grid
```html
<flux:grid />
```

#### flux:outlet
```html
<flux:outlet${1: enabled="1"} />
```

#### flux:variable
```html
<flux:variable name="$1" />
```
---
### \<flux:content.*\>

#### flux:content.get
```html
<flux:content.get area="$1"${3: limit="$2"}${5: offset="$4"}${7: order="'${6:sorting}'"}${9: sortDirection="'${8:ASC}'"}${11: as="$10"}${13: loadRegister="$12"}${15: render="${14:1}"} />
```

#### flux:content.render
```html
<flux:content.render area="$1"${3: limit="$2"}${5: offset="$4"}${7: order="'${6:sorting}'"}${9: sortDirection="'${8:ASC}'"}${11: as="$10"}${13: loadRegister="$12"}${15: render="${14:1}"} />
```
---
### \<flux:field.*\>

#### flux:field.inline.fal
```html
<flux:field.inline.fal name="$1" label="$2"${3: required="1"}${4: multiple="0"}${6: minItems="$5"}${8: maxItems="$7"}${9: collapseAll="0"}${10: expandSingle="0"} allowedExtensions="${11:jpg,jpeg,png,svg}" />
```

#### flux:field.tree.category*
```html
<flux:field.tree.category name="$1" label="$2"${3: required="1"}${4: multiple="0"}${6: minItems="$5"}${8: maxItems="$7"}${9: showThumbs="1"}${10: expandAll="1"} />
```

#### flux:field.checkbox
```html
<flux:field.checkbox name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${7: clear="1"} />
```

#### flux:field.controllerActions*
```html
<flux:field.controllerActions name="$1" label="$2" required="1" exclude="1"  extensionName="NULL" controllerExtensionName="NULL" pluginName="NULL" controllerName="NULL" actions="{foo: 'bar'}" />
```

#### flux:field.custom*
```html
<flux:field.custom name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${7: clear="1"}${9: userFunc="${8:FluidTYPO3\\Flux\\UserFunction\\HtmlOutput->renderField}"} />
  ```

#### flux:field.file
```html
<flux:field.file name="$1" label="$2"${4: required="1"}${5: multiple="1"}${7: minItems="$6"}${9: maxItems="$8"}${11: allowed="${10:jpg,png,gif,svg}"}${12: showThumbnails="1"}${13: useFalRelation="1"} />
```

#### flux:field.inline*
```html
<flux:field.inline name="$1" label="$2" eextensionName="NULL" table="NULL" />
```

#### flux:field.input
```html
<flux:field.input name="$1" label="$2"${4: default="$3"}${5: required="1"}${7: eval="${6:'trim'}"}${9: maxCharacters="$8"}${11: placeholder="$10"} />
```

#### flux:field.multiRelation*
```html
<flux:field.multiRelation name="$1" label="$2" />
```

#### flux:field.none
```html
<flux:field.none name="$1" label="$2" default="$3" />
```

#### flux:field.radio
```html
<flux:field.radio name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"} items="{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}" />
```

#### flux:field.relation*
```html
<flux:field.relation name="$1" label="$2" />
```

#### flux:field.select
```html
<flux:field.select name="$1" label="$2"${4: default="$3"}${5: required="1"}${6: requestUpdate="1"}${8: renderType="${7|selectSingle,selectSingleBox,selectCheckBox,selectMultipleSideBySide,selectTree|}${10: size="$9"}${12: maxItems="$11"} items="{0:{0:'One',1:'0'},1:{0:'Two',1:'1'}}" />
```

#### flux:field.text
```html
<flux:field.text name="$1" label="$2"${4: required="1"}${6: validate="'${5:trim}'"}${7: enableRichText="1"} />
```

#### flux:field.tree*
```html
<flux:field.tree name="$1" label="$2"${4: required="1"} />
```

#### flux:field.userFunc*
```html
<flux:field.userFunc name="$1" label="$2"${5: extensionName="$4"} userFunc="$6" />
```
---
### \<flux:form.*\>

#### flux:form.option.group

```html
<flux:form.option.group value="$1" />
```

#### flux:form.option.icon
```html
<flux:form.option.icon value="/typo3conf/ext/$1/Resources/Public/Icons/${2:icon.svg}" />
```

#### flux:form.option.sorting
```html
<flux:form.option.sorting value="$1" />
```

#### flux:form.option.static
```html
<flux:form.option.static value="${1:1}" />
```

#### flux:form.container
```html
<flux:form.container name="$1" label="$2" />
```

#### flux:form.content
```html
<flux:form.content name="$1" label="$2" />
```

#### flux:form.data
```html
<flux:form.data table="$1" field="$2" uid="$3" record="${4:{foo: 'bar'}}" as="$5" />
```

#### flux:form.object
```html
<flux:form.object name="$1" label="$2" />
```

#### flux:form.option
```html
<flux:form.option name="$1" value="$2" />
```

#### flux:form.render
```html
<flux:form.render form="$1" />
```

#### flux:form.section
```html
<flux:form.section name="$1" label="$2" />
```

#### flux:form.sheet
```html
<flux:form.sheet name="$1" label="$2"${4: description="$3"}${6: shortDescription="$5"} />
```

#### flux:form.variable
```html
<flux:form.variable name="$1" value="$2" />
```
---
### \<flux:grid.*\>

#### flux:grid.column
```html
<flux:grid.column name="$1" label="$2" colPos="$3"${5: colspan="$4"}${7: rowspan="$6"}${9: style="$8"} />
```

#### flux:grid.row
```html
<flux:grid.row name="$1" label="$2" />
```
---
### \<flux:outlet.*\>

#### flux:outlet.argument
```html
<flux:outlet.argument name="$1" type="$2" />
```

#### flux:outlet.form
```html
<flux:outlet.form name="$1" action="$2" controller="$3" extensionName="$4" pluginName="$5" pageUid="$6" />
```

#### flux:outlet.validate
```html
<flux:outlet.validate type="$1"${3: options="$2"} />
```
---
### \<flux:pipe.*\>

#### flux:pipe.controller
```html
<flux:pipe.controller direction="$1" action="$2" controller="$3" extensionName="$4" />
```

#### flux:pipe.email
```html
<flux:pipe.email direction="$1" body="$2" bodySection="$3" subject="$4" recipient="$5" sender="$6" />
```

#### flux:pipe.flashMessage
```html
<flux:pipe.flashMessage direction="$1" message="$2" title="'$3'" severity="$4"${5: storeInSession="1"} />
```

#### flux:pipe.typeConverter
```html
<flux:pipe.typeConverter direction="$1" targetType="$2" typeConverter="$3" />
```
---
### \<flux:wizard.*\>

#### flux:wizard.add
```html
<flux:wizard.add label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pid="$6" setValue="'prepend'" />
```

#### flux:wizard.colorPicker
```html
<flux:wizard.colorPicker label="$1" dim="'${2:20x20}'" width="$3" height="$4" exampleImg="'${5:EXT:flux/Resources/Public/Icons/ColorWheel.png}'" />
```

#### flux:wizard.edit
```html
<flux:wizard.edit label="$1"${2: hideParent="1"}${4: extensionName="$3"} width="$5" height="$6"${7: openOnlyIfSelected="1"} />
```

#### flux:wizard.link
```html
<flux:wizard.link label="$1"${2: hideParent="1"}${4: extensionName="$3"} activeTab="'${5:file}'" width="$6" height="$7"${9: allowedExtensions="$8"} />
```

#### flux:wizard.list
```html
<flux:wizard.list label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pid="$6" width="$7" height="$8" />
```

#### flux:wizard.select
```html
<flux:wizard.select label="$1"${2: hideParent="1"}${4: extensionName="$3"} mode="'${5:substitution}'" items="$6" />
```

#### flux:wizard.slider
```html
<flux:wizard.slider label="$1"${2: hideParent="1"}${4: extensionName="$3"} mode="'${5:substitution}'" steps="$6" width="$7" />
```

#### flux:wizard.suggest
```html
<flux:wizard.suggest label="$1"${2: hideParent="1"}${4: extensionName="$3"} table="$5" pidList="'$6'" pidDepth="$7" minimumCharacters="$8" maxPathTitleLength="$9"${10: searchWholePhrase="1"} searchCondition="'$11'"${13: cssClass="'$12'"}${15: receiverClass="'$14'"}${17: renderFunc="'$16'"} />
```

## Templates overview

#### flux-ce-template
```html
<div xmlns="http://www.w3.org/1999/xhtml" lang="en"
  xmlns:f="http://typo3.org/ns/TYPO3/Fluid/ViewHelpers"
  xmlns:flux="http://typo3.org/ns/FluidTYPO3/Flux/ViewHelpers"
  xmlns:v="http://typo3.org/ns/FluidTYPO3/Vhs/ViewHelpers">

  <f:layout name="Content" />

  <f:section name="Configuration">
    <flux:form
      id="${1:${TM_FILENAME_BASE/(^.)/${1:/downcase}/}}"
      label="${2:$TM_FILENAME_BASE}"
      description="$${3:$TM_FILENAME_BASE}"
    >
      <flux:form.option name="group" value="${4:Flux}" />
      <flux:form.option name="icon" value="EXT:$5/Resources/Public/Icons/Content/Standard.svg" />
      $6
    </flux:form>
  </f:section>

  <f:section name="Preview">
    <h3>${2:$TM_FILENAME_BASE}</h3>
  </f:section>

  <f:section name="Main">
    $7
  </f:section>
</div>
```

## Source

All snippets have been taken from [fluidtypo3.org](https://fluidtypo3.org/viewhelpers/flux/master.html) ViewHelper reference<br>

## Recommendations

Works perfectly together with other TYPO3 snippet extension<br>
https://github.com/MrSilaz/typo3snippets<br>
https://github.com/febLey/vscode-typo3-vhs-snippets

## License

[GNU General Public License (GPL), Version 2.0](http://www.gnu.org/licenses/gpl-2.0.html)
