

# Slot: payor 



URI: [sow:payor](https://w3id.org/collabri/sow/payor)
Alias: payor

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Payment](Payment.md) | Payment obligation tied to milestone acceptance |  no  |






## Properties

* Range: [PayorParty](PayorParty.md)

* Required: True




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:payor |
| native | sow:payor |




## LinkML Source

<details>
```yaml
name: payor
from_schema: https://w3id.org/collabri/sow
rank: 1000
alias: payor
owner: Payment
domain_of:
- Payment
range: PayorParty
required: true

```
</details>