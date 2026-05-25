

# Slot: authored_by 



URI: [pav:authoredBy](http://purl.org/pav/authoredBy)
Alias: authored_by

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Milestone](Milestone.md) | A milestone is a collection of subtasks (linked via Subtask |  no  |
| [Activity](Activity.md) | An event-type deliverable (training, workshop, presentation) |  no  |
| [Standard](Standard.md) | A normative or internal standard, classified by subtype (ADMS-aligned) |  no  |
| [Software](Software.md) |  |  no  |
| [Deliverable](Deliverable.md) | Artifact produced by a single subtask |  no  |
| [Method](Method.md) | A method deliverable, modeled as a prov:Plan |  no  |
| [Task](Task.md) | Thematic bucket of work, possibly spanning the full award |  no  |
| [NarrativeDocument](NarrativeDocument.md) | Policy, SOP, report, recommendation, publication, progress-report blurb, etc |  no  |
| [Subtask](Subtask.md) | A step toward completion of a Task |  no  |
| [Versioned](Versioned.md) | Per-element version metadata, aligned with PAV and PROV |  no  |
| [TaskTeam](TaskTeam.md) | Root of a SOW |  no  |
| [Data](Data.md) | Dataset, spreadsheet, or other structured-data artifact |  no  |






## Properties

* Range: [Uriorcurie](Uriorcurie.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | pav:authoredBy |
| native | sow:authored_by |




## LinkML Source

<details>
```yaml
name: authored_by
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: pav:authoredBy
alias: authored_by
owner: Versioned
domain_of:
- Versioned
range: uriorcurie
multivalued: true

```
</details>