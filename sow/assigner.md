

# Slot: assigner 


_Party imposing the obligation._





URI: [odrl:assigner](http://www.w3.org/ns/odrl/2/assigner)
Alias: assigner

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
| self | odrl:assigner |
| native | sow:assigner |




## LinkML Source

<details>
```yaml
name: assigner
description: Party imposing the obligation.
from_schema: https://w3id.org/collabri/sow
rank: 1000
slot_uri: odrl:assigner
alias: assigner
owner: Obligation
domain_of:
- Obligation
range: Party
inlined: true

```
</details>