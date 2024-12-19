# Extension: onBackgroundColor

URL for this extension:

```
https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md
```

Status: draft. Extension maintained by: Pistevo Decision

onBackgroundColor: The color for text on a background for a questionnaire item or header.

Context of Use: Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item

## Extension Content

### Summary

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)      | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                                   |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **onBackgroundColor**                              |                                                     | 0..1                                                | [string](https://hl7.org/fhir/R4/datatypes.html#string) | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md<br>onBackgroundColor: The color for text on a background for a questionnaire item or header.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |

---

### Full Structure

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)      | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                                   |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **extension**                                      |                                                     | 0..1                                                | Extension                                               | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md<br>onBackgroundColor: The color for text on a background for a questionnaire item or header.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |
| &nbsp;&nbsp;└ **extension**                        | I                                                   | 0..0                                                |                                                         |                                                                                                                                                                                                                                                                                                           |
| &nbsp;&nbsp;└ **url**                              |                                                     | 1..1                                                | [uri](https://hl7.org/fhir/R4/datatypes.html#uri)       | "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md"                                                                                                                                                                                    |
| &nbsp;&nbsp;└ **value[x]**                         | I                                                   | 1..1                                                | [string](https://hl7.org/fhir/R4/datatypes.html#string) | Value of extension                                                                                                                                                                                                                                                                                        |

### XML Template

```xml
<!-- iconData -->

<extension xmlns="http://hl7.org/fhir"
     url="https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md" >
  <!-- from Element: extension -->
 <valueString value="[string]"/><!-- 1..1 Value of extension -->
</extension>
```

### JSON Template

```
{ // iconData
  // from Element: extension
    "extension" : [ //  sliced by value:url  in the specified order, Open ]
    "url" : "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionaire-onBackgroundColor.md", // R!
    "valueString" : "<string>" // C? R! Value of extension
  }
```

#### Contraints

- **ele-1**: All FHIR elements must have a @value or children (xpath: `@value|f:*|h:div`)
- **ext-1**: Must have either extensions or value[x], not both (xpath: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), 'value')])`)
- **ele-1**: On Extension.extension: All FHIR elements must have a @value or children (xpath on Extension.extension: `@value|f:*|h:div`)
- **ext-1**: On Extension.extension: Must have either extensions or value[x], not both (xpath on Extension.extension: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), "value")])`)
- **ele-1**: On Extension.value[x]: All FHIR elements must have a @value or children (xpath on Extension.value[x]: `@value|f:*|h:div`)
