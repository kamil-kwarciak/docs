# Path Picker

**wcm/dialogs/components/pathpicker**

## Description

Path picker is an input that allows the user pick path of resource from repository or to introduce external links. If the value starts with `/` the path picker will autosuggest possible values.

![PathPicker](pathpicker.png)

## Properties

- **name** -  `string` (required)  
    Form field name

- **label** - `string`  
    Display label value

- **required** - `string`  
    Indicates if field value is mandatory

- **rootPath** - `string`  
    Root path of pathpicker

- **forceRootPath** - `string` (if not defined `false`)  
    Indicates whether the input value should start with the value defined in `rootPath` property

- **removeIfEmpty** - `string` (if not defined `false`)  
    Indicates if property in JCR will be removed, if contains empty String, or will be kept with that value

- **description** - `string`  
    Display description value as a tooltip

## Example

```json
"link": {
  "sling:resourceType": "wcm/dialogs/components/pathpicker",
  "rootPath": "/content",
  "name": "link",
  "label": "URL",
  "forceRootPath": true
}
```
