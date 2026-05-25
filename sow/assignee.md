

# Slot: assignee 


_Party bound by the obligation._





URI: [odrl:assignee](http://www.w3.org/ns/odrl/2/assignee)
Alias: assignee

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Obligation](Obligation.md) | Abstract base for any contractual duty (ODRL pattern) |  no  |
| [ReportingObligation](ReportingObligation.md) | Recurring reporting duty (quarterly progress report, annual technical report,... |  no  |
| [Payment](Payment.md) | Payment obligation tied to milestone acceptance |  no  |






## Properties

* Range: [Party](Party.md)




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | odrl:assignee |
| native | sow:assignee |




## LinkML Source

<details>
```yaml
name: assignee
description: Party bound by the obligation.
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: odrl:assignee
alias: assignee
owner: Obligation
domain_of:
- Obligation
range: Party
inlined: true

```
</details>