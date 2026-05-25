

# Slot: contributors 



URI: [sow:contributors](https://w3id.org/collabri/sow/contributors)
Alias: contributors

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Activity](Activity.md) | An event-type deliverable (training, workshop, presentation) |  no  |
| [Standard](Standard.md) | A normative or internal standard, classified by subtype (ADMS-aligned) |  no  |
| [Software](Software.md) |  |  no  |
| [Deliverable](Deliverable.md) | Artifact produced by a single subtask |  no  |
| [Method](Method.md) | A method deliverable, modeled as a prov:Plan |  no  |
| [NarrativeDocument](NarrativeDocument.md) | Policy, SOP, report, recommendation, publication, progress-report blurb, etc |  no  |
| [Data](Data.md) | Dataset, spreadsheet, or other structured-data artifact |  no  |






## Properties

* Range: [Contribution](Contribution.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:contributors |
| native | sow:contributors |




## LinkML Source

<details>
```yaml
name: contributors
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: contributors
owner: Deliverable
domain_of:
- Deliverable
range: Contribution
multivalued: true
inlined: true
inlined_as_list: true

```
</details>