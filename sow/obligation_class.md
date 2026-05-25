

# Slot: obligation_class 


_Discriminator for the concrete Obligation subclass. Auto-set by subclasses; instance YAML should set this to the subclass name (e.g., Payment, ReportingObligation)._





URI: [sow:obligation_class](https://w3id.org/collabri/sow/obligation_class)
Alias: obligation_class

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Obligation](Obligation.md) | Abstract base for any contractual duty (ODRL pattern) |  no  |
| [ReportingObligation](ReportingObligation.md) | Recurring reporting duty (quarterly progress report, annual technical report,... |  no  |
| [Payment](Payment.md) | Payment obligation tied to milestone acceptance |  no  |






## Properties

* Range: [String](String.md)




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:obligation_class |
| native | sow:obligation_class |




## LinkML Source

<details>
```yaml
name: obligation_class
description: Discriminator for the concrete Obligation subclass. Auto-set by subclasses;
  instance YAML should set this to the subclass name (e.g., Payment, ReportingObligation).
from_schema: https://w3id.org/collabri/sow
rank: 1000
designates_type: true
alias: obligation_class
owner: Obligation
domain_of:
- Obligation
range: string

```
</details>