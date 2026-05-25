

# Class: Method 


_A method deliverable, modeled as a prov:Plan. Methods are typically managed as controlled documents (e.g., in Collabri) where each document and section is under change control. This class carries pointers and version metadata; full OBI protocol modeling is intentionally out of scope._





URI: [prov:Plan](http://www.w3.org/ns/prov#Plan)





```mermaid
 classDiagram
    class Method
    click Method href "../Method/"
      Deliverable <|-- Method
        click Deliverable href "../Deliverable/"
      
      Method : authored_by
        
      Method : category
        
          
    
        
        
        Method --> "1" DeliverableCategory : category
        click DeliverableCategory href "../DeliverableCategory/"
    

        
      Method : collabri_doc_id
        
      Method : contractual_status
        
          
    
        
        
        Method --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Method : contributors
        
          
    
        
        
        Method --> "*" Contribution : contributors
        click Contribution href "../Contribution/"
    

        
      Method : created_on
        
      Method : current_version
        
      Method : delivered_date
        
      Method : description
        
      Method : due_date
        
      Method : id
        
      Method : name
        
      Method : performance_status
        
          
    
        
        
        Method --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Method : previous_version
        
      Method : protocol_url
        
      Method : section_ref
        
      Method : uri
        
      Method : version
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * [Deliverable](Deliverable.md) [ [Versioned](Versioned.md) [Trackable](Trackable.md)]
        * **Method**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [collabri_doc_id](collabri_doc_id.md) | 0..1 <br/> [String](String.md) | Controlled-document identifier in Collabri | direct |
| [section_ref](section_ref.md) | 0..1 <br/> [String](String.md) | Section under change control, if scoped narrower than the full doc | direct |
| [protocol_url](protocol_url.md) | 0..1 <br/> [uri](uri.md) |  | direct |
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
| self | prov:Plan |
| native | sow:Method |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Method
description: A method deliverable, modeled as a prov:Plan. Methods are typically managed
  as controlled documents (e.g., in Collabri) where each document and section is under
  change control. This class carries pointers and version metadata; full OBI protocol
  modeling is intentionally out of scope.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(method)
    equals_string: method
attributes:
  collabri_doc_id:
    name: collabri_doc_id
    description: Controlled-document identifier in Collabri.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Method
  section_ref:
    name: section_ref
    description: Section under change control, if scoped narrower than the full doc.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Method
  protocol_url:
    name: protocol_url
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Method
    range: uri
class_uri: prov:Plan

```
</details>

### Induced

<details>
```yaml
name: Method
description: A method deliverable, modeled as a prov:Plan. Methods are typically managed
  as controlled documents (e.g., in Collabri) where each document and section is under
  change control. This class carries pointers and version metadata; full OBI protocol
  modeling is intentionally out of scope.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(method)
    equals_string: method
attributes:
  collabri_doc_id:
    name: collabri_doc_id
    description: Controlled-document identifier in Collabri.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: collabri_doc_id
    owner: Method
    domain_of:
    - Method
    range: string
  section_ref:
    name: section_ref
    description: Section under change control, if scoped narrower than the full doc.
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: section_ref
    owner: Method
    domain_of:
    - Method
    range: string
  protocol_url:
    name: protocol_url
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: protocol_url
    owner: Method
    domain_of:
    - Method
    range: uri
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    ifabsent: string(method)
    alias: category
    owner: Method
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
    equals_string: method
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: due_date
    owner: Method
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: delivered_date
    owner: Method
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    alias: uri
    owner: Method
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contributors
    owner: Method
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
    owner: Method
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
    owner: Method
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
    owner: Method
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Method
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Method
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Method
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Method
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
    owner: Method
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
    owner: Method
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
    owner: Method
    domain_of:
    - NamedThing
    range: string
class_uri: prov:Plan

```
</details>