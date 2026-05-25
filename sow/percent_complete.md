

# Slot: percent_complete 


_For partial-completion payable subtasks (e.g., reports paid in stages), the current percent complete against the subtask's scope._





URI: [sow:percent_complete](https://w3id.org/collabri/sow/percent_complete)
Alias: percent_complete

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Subtask](Subtask.md) | A step toward completion of a Task |  no  |






## Properties

* Range: [Float](Float.md)

* Minimum Value: 0

* Maximum Value: 100




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:percent_complete |
| native | sow:percent_complete |




## LinkML Source

<details>
```yaml
name: percent_complete
description: For partial-completion payable subtasks (e.g., reports paid in stages),
  the current percent complete against the subtask's scope.
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: percent_complete
owner: Subtask
domain_of:
- Subtask
range: float
minimum_value: 0
maximum_value: 100

```
</details>