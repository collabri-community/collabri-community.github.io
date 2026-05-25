

# Class: Standard 


_A normative or internal standard, classified by subtype (ADMS-aligned)._





URI: [dcterms:Standard](http://purl.org/dc/terms/Standard)





```mermaid
 classDiagram
    class Standard
    click Standard href "../Standard/"
      Deliverable <|-- Standard
        click Deliverable href "../Deliverable/"
      
      Standard : authored_by
        
      Standard : category
        
          
    
        
        
        Standard --> "1" DeliverableCategory : category
        click DeliverableCategory href "../DeliverableCategory/"
    

        
      Standard : contractual_status
        
          
    
        
        
        Standard --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Standard : contributors
        
          
    
        
        
        Standard --> "*" Contribution : contributors
        click Contribution href "../Contribution/"
    

        
      Standard : created_on
        
      Standard : current_version
        
      Standard : delivered_date
        
      Standard : description
        
      Standard : due_date
        
      Standard : id
        
      Standard : name
        
      Standard : performance_status
        
          
    
        
        
        Standard --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Standard : previous_version
        
      Standard : standard_body
        
      Standard : standard_subtype
        
          
    
        
        
        Standard --> "1" StandardSubtype : standard_subtype
        click StandardSubtype href "../StandardSubtype/"
    

        
      Standard : uri
        
      Standard : version
        
      Standard : version_label
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * [Deliverable](Deliverable.md) [ [Versioned](Versioned.md) [Trackable](Trackable.md)]
        * **Standard**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [standard_subtype](standard_subtype.md) | 1 <br/> [StandardSubtype](StandardSubtype.md) |  | direct |
| [standard_body](standard_body.md) | 0..1 <br/> [String](String.md) | Organization stewarding the standard, if external | direct |
| [version_label](version_label.md) | 0..1 <br/> [String](String.md) |  | direct |
| [category](category.md) | 1 <br/> [DeliverableCategory](DeliverableCategory.md) |  | [Deliverable](Deliverable.md) |
| [due_date](due_date.md) | 0..1 <br/> [Date](Date.md) |  | [Deliverable](Deliverable.md) |
| [delivered_date](delivered_date.md) | 0..1 <br/> [Date](Date.md) |  | [Deliverable](Deliverable.md) |
| [uri](uri.md) | 0..1 <br/> [uri](uri.md) |  | [Deliverable](Deliverable.md) |
| [contributors](contributors.md) | * <br/> [Contribution](Contribution.md) |  | [Deliverable](Deliverable.md) |
| [version](version.md) | 0..1 <br/> [String](String.md) | Semantic version of this element | [Versioned](Versioned.md) |
| [previous_version](previous_version.md) | 0..1 <br/> [Uriorcurie](Uriorcurie.md) | IRI of the immediately prior version of this element | [Versioned](Versioned.md) |
| [current_version](current_version.md) | 0..1 <br/> [Boolean](Boolean.md) | True iff this is the current accepted version of the element | [Versioned](Versioned.md) |
| [created_on](created_on.md) | 0..1 <br/> [Date](Date.md) |  | [Versioned](Versioned.md) |
| [authored_by](authored_by.md) | * <br/> [Uriorcurie](Uriorcurie.md) |  | [Versioned](Versioned.md) |
| [contractual_status](contractual_status.md) | 1 <br/> [ContractualStatus](ContractualStatus.md) |  | [Trackable](Trackable.md) |
| [performance_status](performance_status.md) | 0..1 <br/> [PerformanceStatus](PerformanceStatus.md) |  | [Trackable](Trackable.md) |
| [id](id.md) | 1 <br/> [String](String.md) | Stable ID; together with version forms the element IRI | [NamedThing](NamedThing.md) |
| [name](name.md) | 1 <br/> [String](String.md) |  | [NamedThing](NamedThing.md) |
| [description](description.md) | 0..1 <br/> [String](String.md) |  | [NamedThing](NamedThing.md) |










## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | dcterms:Standard |
| native | sow:Standard |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Standard
description: A normative or internal standard, classified by subtype (ADMS-aligned).
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(standard)
    equals_string: standard
attributes:
  standard_subtype:
    name: standard_subtype
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Standard
    range: StandardSubtype
    required: true
  standard_body:
    name: standard_body
    description: Organization stewarding the standard, if external.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Standard
  version_label:
    name: version_label
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Standard
class_uri: dcterms:Standard

```
</details>

### Induced

<details>
```yaml
name: Standard
description: A normative or internal standard, classified by subtype (ADMS-aligned).
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(standard)
    equals_string: standard
attributes:
  standard_subtype:
    name: standard_subtype
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: standard_subtype
    owner: Standard
    domain_of:
    - Standard
    range: StandardSubtype
    required: true
  standard_body:
    name: standard_body
    description: Organization stewarding the standard, if external.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: standard_body
    owner: Standard
    domain_of:
    - Standard
    range: string
  version_label:
    name: version_label
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: version_label
    owner: Standard
    domain_of:
    - Standard
    range: string
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    ifabsent: string(standard)
    alias: category
    owner: Standard
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
    equals_string: standard
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: due_date
    owner: Standard
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: delivered_date
    owner: Standard
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    alias: uri
    owner: Standard
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contributors
    owner: Standard
    domain_of:
    - Deliverable
    range: Contribution
    multivalued: true
    inlined: true
    inlined_as_list: true
  version:
    name: version
    description: Semantic version of this element.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:version
    alias: version
    owner: Standard
    domain_of:
    - Versioned
    range: string
  previous_version:
    name: previous_version
    description: IRI of the immediately prior version of this element.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:previousVersion
    alias: previous_version
    owner: Standard
    domain_of:
    - Versioned
    range: uriorcurie
  current_version:
    name: current_version
    description: True iff this is the current accepted version of the element.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:hasCurrentVersion
    alias: current_version
    owner: Standard
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Standard
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Standard
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Standard
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Standard
    domain_of:
    - Trackable
    range: PerformanceStatus
  id:
    name: id
    description: Stable ID; together with version forms the element IRI.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcterms:identifier
    identifier: true
    alias: id
    owner: Standard
    domain_of:
    - NamedThing
    - Approval
    - ChangeProposal
    - Change
    range: string
    required: true
  name:
    name: name
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: schema:name
    alias: name
    owner: Standard
    domain_of:
    - NamedThing
    range: string
    required: true
  description:
    name: description
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcterms:description
    alias: description
    owner: Standard
    domain_of:
    - NamedThing
    range: string
class_uri: dcterms:Standard

```
</details>