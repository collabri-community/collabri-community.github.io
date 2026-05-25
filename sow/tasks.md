

# Slot: tasks 



URI: [sow:tasks](https://w3id.org/collabri/sow/tasks)
Alias: tasks

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [TaskTeam](TaskTeam.md) | Root of a SOW |  no  |






## Properties

* Range: [Task](Task.md)

* Multivalued: True

* Required: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:tasks |
| native | sow:tasks |




## LinkML Source

<details>
```yaml
name: tasks
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: tasks
owner: TaskTeam
domain_of:
- TaskTeam
range: Task
required: true
multivalued: true
inlined: true
inlined_as_list: true

```
</details>