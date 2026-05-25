

# Slot: obligations 


_Non-payment obligations attached at the agreement level (reporting cadence, data rights, IP terms, etc.). Payments live on milestones rather than here, but both are Obligations._





URI: [odrl:obligation](http://www.w3.org/ns/odrl/2/obligation)
Alias: obligations

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [TaskTeam](TaskTeam.md) | Root of a SOW |  no  |






## Properties

* Range: [Obligation](Obligation.md)

* Multivalued: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | odrl:obligation |
| native | sow:obligations |




## LinkML Source

<details>
```yaml
name: obligations
description: Non-payment obligations attached at the agreement level (reporting cadence,
  data rights, IP terms, etc.). Payments live on milestones rather than here, but
  both are Obligations.
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: odrl:obligation
alias: obligations
owner: TaskTeam
domain_of:
- TaskTeam
range: Obligation
multivalued: true
inlined: true
inlined_as_list: true

```
</details>