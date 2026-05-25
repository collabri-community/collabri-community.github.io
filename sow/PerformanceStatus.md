# Enum: PerformanceStatus 




_Execution state, orthogonal to contractual status._



URI: [sow:PerformanceStatus](https://w3id.org/collabri/sow/PerformanceStatus)

## Permissible Values

| Value | Meaning | Description |
| --- | --- | --- |
| not_started | None |  |
| in_progress | None |  |
| blocked | None |  |
| completed | None |  |
| canceled | None |  |




## Slots

| Name | Description |
| ---  | --- |
| [performance_status](performance_status.md) |  |





## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow






## LinkML Source

<details>
```yaml
name: PerformanceStatus
description: Execution state, orthogonal to contractual status.
from_schema: https://w3id.org/collabri/sow
rank: 1000
permissible_values:
  not_started:
    text: not_started
  in_progress:
    text: in_progress
  blocked:
    text: blocked
  completed:
    text: completed
  canceled:
    text: canceled

```
</details>