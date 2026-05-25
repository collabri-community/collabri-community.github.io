

# Slot: category 



URI: [sow:category](https://w3id.org/collabri/sow/category)
Alias: category

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Activity](Activity.md) | An event-type deliverable (training, workshop, presentation) |  yes  |
| [Standard](Standard.md) | A normative or internal standard, classified by subtype (ADMS-aligned) |  yes  |
| [Software](Software.md) |  |  yes  |
| [Deliverable](Deliverable.md) | Artifact produced by a single subtask |  no  |
| [Method](Method.md) | A method deliverable, modeled as a prov:Plan |  yes  |
| [NarrativeDocument](NarrativeDocument.md) | Policy, SOP, report, recommendation, publication, progress-report blurb, etc |  yes  |
| [Data](Data.md) | Dataset, spreadsheet, or other structured-data artifact |  yes  |






## Properties

* Range: [DeliverableCategory](DeliverableCategory.md)

* Required: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:category |
| native | sow:category |




## LinkML Source

<details>
```yaml
name: category
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: category
owner: Deliverable
domain_of:
- Deliverable
range: DeliverableCategory
required: true

```
</details>