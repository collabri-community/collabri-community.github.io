

# Slot: milestones 


_Milestones for this SOW. Subtasks point at milestones by ID; a milestone is the contractual acceptance event that gates payment for its referencing subtasks._





URI: [sow:milestones](https://w3id.org/collabri/sow/milestones)
Alias: milestones

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [TaskTeam](TaskTeam.md) | Root of a SOW |  no  |






## Properties

* Range: [Milestone](Milestone.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:milestones |
| native | sow:milestones |




## LinkML Source

<details>
```yaml
name: milestones
description: Milestones for this SOW. Subtasks point at milestones by ID; a milestone
  is the contractual acceptance event that gates payment for its referencing subtasks.
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: milestones
owner: TaskTeam
domain_of:
- TaskTeam
range: Milestone
multivalued: true
inlined: true
inlined_as_list: true

```
</details>