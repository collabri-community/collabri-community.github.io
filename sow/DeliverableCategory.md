# Enum: DeliverableCategory 




_High-level kind of deliverable artifact._



URI: [sow:DeliverableCategory](https://w3id.org/collabri/sow/DeliverableCategory)

## Permissible Values

| Value | Meaning | Description |
| --- | --- | --- |
| narrative_document | iao:0000310 |  |
| software | doap:Project |  |
| data | dcat:Dataset |  |
| standard | dcterms:Standard |  |
| method | prov:Plan |  |
| activity | schema:Event |  |




## Slots

| Name | Description |
| ---  | --- |
| [category](category.md) |  |





## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow






## LinkML Source

<details>
```yaml
name: DeliverableCategory
description: High-level kind of deliverable artifact.
from_schema: https://w3id.org/collabri/sow
rank: 1000
permissible_values:
  narrative_document:
    text: narrative_document
    meaning: iao:0000310
  software:
    text: software
    meaning: doap:Project
  data:
    text: data
    meaning: dcat:Dataset
  standard:
    text: standard
    meaning: dcterms:Standard
  method:
    text: method
    meaning: prov:Plan
  activity:
    text: activity
    meaning: schema:Event

```
</details>