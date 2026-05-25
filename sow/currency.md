

# Slot: currency 



URI: [sow:currency](https://w3id.org/collabri/sow/currency)
Alias: currency

<!-- no inheritance hierarchy -->





## Applicable Classes

| Name | Description | Modifies Slot |
| --- | --- | --- |
| [Money](Money.md) | Monetary amount with currency |  no  |






## Properties

* Range: [String](String.md)




## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | sow:currency |
| native | sow:currency |




## LinkML Source

<details>
```yaml
name: currency
from_schema: https://w3id.org/collabri/sow
rank: 1000
ifabsent: string(USD)
alias: currency
owner: Money
domain_of:
- Money
range: string

```
</details>