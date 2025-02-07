# Extension: svgIcon

URL for this extension:

```
https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md
```

Status: draft. Extension maintained by: Pistevo Decision

The svg string representation of an icon corresponding to a questionnaire item.

Context of Use: Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item

## Extension Content

### Summary

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)      | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                         |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **svgIcon**                                        |                                                     | 0..1                                                | [string](https://hl7.org/fhir/R4/datatypes.html#string) | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md<br>svgIcon: The svg string representation of an icon corresponding to a questionnaire item.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |

---

### Full Structure

| [Name](https://hl7.org/fhir/R4/formats.html#table) | [Flags](https://hl7.org/fhir/R4/formats.html#table) | [Card.](https://hl7.org/fhir/R4/formats.html#table) | [Type](https://hl7.org/fhir/R4/formats.html#table)      | [Description & Constraints](https://hl7.org/fhir/R4/formats.html#table)                                                                                                                                                                                                                         |
| -------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **extension**                                      |                                                     | 0..1                                                | Extension                                               | URL = https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md<br>svgIcon: The svg string representation of an icon corresponding to a questionnaire item.<br><br>Use on Element ID Questionnaire.item or Element ID Questionnaire.item.item |
| &nbsp;&nbsp;└ **extension**                        | I                                                   | 0..0                                                |                                                         |                                                                                                                                                                                                                                                                                                 |
| &nbsp;&nbsp;└ **url**                              |                                                     | 1..1                                                | [uri](https://hl7.org/fhir/R4/datatypes.html#uri)       | "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md"                                                                                                                                                                                   |
| &nbsp;&nbsp;└ **value[x]**                         | I                                                   | 1..1                                                | [string](https://hl7.org/fhir/R4/datatypes.html#string) | Value of extension                                                                                                                                                                                                                                                                              |

### XML Template

```xml
<!-- svgIcon -->

<extension xmlns="http://hl7.org/fhir"
     url="https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md" >
  <!-- from Element: extension -->
 <valueString value="[string]"/><!-- 1..1 Value of extension -->
</extension>
```

### JSON Template

```JSON
{ // svgIcon
  // from Element: extension
    "extension" : [ //  sliced by value:url  in the specified order, Open ]
    "url" : "https://github.com/pistevo-decision/fhir-extension/blob/main/structure_definitions/questionnaire-svgIcon.md", // R!
    "valueString" : "<string>" // C? R! Value of extension
  }
```

#### Contraints

- **ele-1**: All FHIR elements must have a @value or children (xpath: `@value|f:*|h:div`)
- **ext-1**: Must have either extensions or value[x], not both (xpath: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), 'value')])`)
- **ele-1**: On Extension.extension: All FHIR elements must have a @value or children (xpath on Extension.extension: `@value|f:*|h:div`)
- **ext-1**: On Extension.extension: Must have either extensions or value[x], not both (xpath on Extension.extension: `exists(f:extension)!=exists(f:*[starts-with(local-name(.), "value")])`)
- **ele-1**: On Extension.value[x]: All FHIR elements must have a @value or children (xpath on Extension.value[x]: `@value|f:*|h:div`)
