

# Class: Data 


_Dataset, spreadsheet, or other structured-data artifact._





URI: [dcat:Dataset](http://www.w3.org/ns/dcat#Dataset)





```mermaid
 classDiagram
    class Data
    click Data href "../Data/"
      Deliverable <|-- Data
        click Deliverable href "../Deliverable/"
      
      Data : authored_by
        
      Data : category
        
          
    
        
        
        Data --> "1" DeliverableCategory : category
        click DeliverableCategory href "../DeliverableCategory/"
    

        
      Data : contractual_status
        
          
    
        
        
        Data --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Data : contributors
        
          
    
        
        
        Data --> "*" Contribution : contributors
        click Contribution href "../Contribution/"
    

        
      Data : created_on
        
      Data : current_version
        
      Data : delivered_date
        
      Data : description
        
      Data : distribution_url
        
      Data : due_date
        
      Data : format
        
      Data : id
        
      Data : name
        
      Data : performance_status
        
          
    
        
        
        Data --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Data : previous_version
        
      Data : record_count
        
      Data : uri
        
      Data : version
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * [Deliverable](Deliverable.md) [ [Versioned](Versioned.md) [Trackable](Trackable.md)]
        * **Data**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [format](format.md) | 0..1 <br/> [String](String.md) |  | direct |
| [record_count](record_count.md) | 0..1 <br/> [Integer](Integer.md) |  | direct |
| [distribution_url](distribution_url.md) | 0..1 <br/> [uri](uri.md) |  | direct |
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
| self | dcat:Dataset |
| native | sow:Data |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Data
description: Dataset, spreadsheet, or other structured-data artifact.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(data)
    equals_string: data
attributes:
  format:
    name: format
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcterms:format
    domain_of:
    - Data
  record_count:
    name: record_count
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Data
    range: integer
  distribution_url:
    name: distribution_url
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:downloadURL
    domain_of:
    - Data
    range: uri
class_uri: dcat:Dataset

```
</details>

### Induced

<details>
```yaml
name: Data
description: Dataset, spreadsheet, or other structured-data artifact.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(data)
    equals_string: data
attributes:
  format:
    name: format
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcterms:format
    alias: format
    owner: Data
    domain_of:
    - Data
    range: string
  record_count:
    name: record_count
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: record_count
    owner: Data
    domain_of:
    - Data
    range: integer
  distribution_url:
    name: distribution_url
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:downloadURL
    alias: distribution_url
    owner: Data
    domain_of:
    - Data
    range: uri
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    ifabsent: string(data)
    alias: category
    owner: Data
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
    equals_string: data
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: due_date
    owner: Data
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: delivered_date
    owner: Data
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    alias: uri
    owner: Data
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contributors
    owner: Data
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
    owner: Data
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
    owner: Data
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
    owner: Data
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Data
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Data
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Data
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Data
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
    owner: Data
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
    owner: Data
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
    owner: Data
    domain_of:
    - NamedThing
    range: string
class_uri: dcat:Dataset

```
</details>