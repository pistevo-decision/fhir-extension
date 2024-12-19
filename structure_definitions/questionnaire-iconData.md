# Extension: iconData

URL for this extension:

```
https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md
```

Status: draft. Extension maintained by: Pistevo Decision

The base64Binary representation of an icon corresponding to a questionnaire item.

Context of Use: Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item

## Extension Content

### Summary

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)                  | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                             |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **iconData**                                       |                                                     | 0..1                                                | [base64Binary](https://hl7.org/fhir/R4/datatypes.html#base64Binary) | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md<br>iconData: The base64Binary representation of an icon corresponding to a questionnaire item.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |

---

### Full Structure

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)                  | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                             |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **extension**                                      |                                                     | 0..1                                                | Extension                                                           | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md<br>iconData: The base64Binary representation of an icon corresponding to a questionnaire item.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |
| &nbsp;&nbsp;└ **extension**                        | I                                                   | 0..0                                                |                                                                     |                                                                                                                                                                                                                                                                                                     |
| &nbsp;&nbsp;└ **url**                              |                                                     | 1..1                                                | [uri](https://hl7.org/fhir/R4/datatypes.html#uri)                   | "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md"                                                                                                                                                                                      |
| &nbsp;&nbsp;└ **value[x]**                         | I                                                   | 1..1                                                | [base64Binary](https://hl7.org/fhir/R4/datatypes.html#base64Binary) | Value of extension                                                                                                                                                                                                                                                                                  |

### XML Template

```xml
<!-- iconData -->

<extension xmlns="http://hl7.org/fhir"
     url="https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md" >
  <!-- from Element: extension -->
 <valueBase64Binary value="[string]"/><!-- 1..1 Value of extension -->
</extension>
```

### JSON Template

```
{ // iconData
  // from Element: extension
    "extension" : [ //  sliced by value:url  in the specified order, Open ]
    "url" : "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-iconData.md", // R!
    "valueBase64Binary" : "<string>" // C? R! Value of extension
  }
```

#### Contraints

- **ele-1**: All FHIR elements must have a @value or children (xpath: `@value|f:*|h:div`)
- **ext-1**: Must have either extensions or value[x], not both (xpath: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), 'value')])`)
- **ele-1**: On Extension.extension: All FHIR elements must have a @value or children (xpath on Extension.extension: `@value|f:*|h:div`)
- **ext-1**: On Extension.extension: Must have either extensions or value[x], not both (xpath on Extension.extension: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), "value")])`)
- **ele-1**: On Extension.value[x]: All FHIR elements must have a @value or children (xpath on Extension.value[x]: `@value|f:*|h:div`)
