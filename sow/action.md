

# Slot: action 


_ODRL action term or local action label (e.g., compensate, report)._





URI: [odrl:action](http://www.w3.org/ns/odrl/2/action)
Alias: action

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Obligation](Obligation.md) | Abstract base for any contractual duty (ODRL pattern) |  no  |
| [ReportingObligation](ReportingObligation.md) | Recurring reporting duty (quarterly progress report, annual technical report,... |  yes  |
| [Payment](Payment.md) | Payment obligation tied to milestone acceptance |  yes  |






## Properties

* Range: [String](String.md)




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | odrl:action |
| native | sow:action |




## LinkML Source

<details>
```yaml
name: action
description: ODRL action term or local action label (e.g., compensate, report).
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: odrl:action
alias: action
owner: Obligation
domain_of:
- Obligation
range: string

```
</details>