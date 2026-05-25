

# Slot: description 



URI: [dcterms:description](http://purl.org/dc/terms/description)
Alias: description

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Milestone](Milestone.md) | A milestone is a collection of subtasks (linked via Subtask |  no  |
| [Activity](Activity.md) | An event-type deliverable (training, workshop, presentation) |  no  |
| [Standard](Standard.md) | A normative or internal standard, classified by subtype (ADMS-aligned) |  no  |
| [Software](Software.md) |  |  no  |
| [Person](Person.md) |  |  no  |
| [Deliverable](Deliverable.md) | Artifact produced by a single subtask |  no  |
| [Organization](Organization.md) |  |  no  |
| [Method](Method.md) | A method deliverable, modeled as a prov:Plan |  no  |
| [Task](Task.md) | Thematic bucket of work, possibly spanning the full award |  no  |
| [NarrativeDocument](NarrativeDocument.md) | Policy, SOP, report, recommendation, publication, progress-report blurb, etc |  no  |
| [Subtask](Subtask.md) | A step toward completion of a Task |  no  |
| [TaskTeam](TaskTeam.md) | Root of a SOW |  no  |
| [NamedThing](NamedThing.md) | Base class for any addressable SOW element |  no  |
| [Data](Data.md) | Dataset, spreadsheet, or other structured-data artifact |  no  |






## Properties

* Range: [String](String.md)




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | dcterms:description |
| native | sow:description |




## LinkML Source

<details>
```yaml
name: description
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: dcterms:description
alias: description
owner: NamedThing
domain_of:
- NamedThing
range: string

```
</details>