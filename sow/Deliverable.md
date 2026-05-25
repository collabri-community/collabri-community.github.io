

# Class: Deliverable 


_Artifact produced by a single subtask. Subtypes specialize by category._




* __NOTE__: this is an abstract class and should not be instantiated directly


URI: [frapo:Deliverable](http://purl.org/cerif/frapo/Deliverable)





```mermaid
 classDiagram
    class Deliverable
    click Deliverable href "../Deliverable/"
      Versioned <|-- Deliverable
        click Versioned href "../Versioned/"
      Trackable <|-- Deliverable
        click Trackable href "../Trackable/"
      NamedThing <|-- Deliverable
        click NamedThing href "../NamedThing/"
      

      Deliverable <|-- NarrativeDocument
        click NarrativeDocument href "../NarrativeDocument/"
      Deliverable <|-- Software
        click Software href "../Software/"
      Deliverable <|-- Data
        click Data href "../Data/"
      Deliverable <|-- Standard
        click Standard href "../Standard/"
      Deliverable <|-- Method
        click Method href "../Method/"
      Deliverable <|-- Activity
        click Activity href "../Activity/"
      

      Deliverable : authored_by
        
      Deliverable : category
        
          
    
        
        
        Deliverable --> "1" DeliverableCategory : category
        click DeliverableCategory href "../DeliverableCategory/"
    

        
      Deliverable : contractual_status
        
          
    
        
        
        Deliverable --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Deliverable : contributors
        
          
    
        
        
        Deliverable --> "*" Contribution : contributors
        click Contribution href "../Contribution/"
    

        
      Deliverable : created_on
        
      Deliverable : current_version
        
      Deliverable : delivered_date
        
      Deliverable : description
        
      Deliverable : due_date
        
      Deliverable : id
        
      Deliverable : name
        
      Deliverable : performance_status
        
          
    
        
        
        Deliverable --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Deliverable : previous_version
        
      Deliverable : uri
        
      Deliverable : version
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * **Deliverable** [ [Versioned](Versioned.md) [Trackable](Trackable.md)]
        * [NarrativeDocument](NarrativeDocument.md)
        * [Software](Software.md)
        * [Data](Data.md)
        * [Standard](Standard.md)
        * [Method](Method.md)
        * [Activity](Activity.md)



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [category](category.md) | 1 <br/> [DeliverableCategory](DeliverableCategory.md) |  | direct |
| [due_date](due_date.md) | 0..1 <br/> [Date](Date.md) |  | direct |
| [delivered_date](delivered_date.md) | 0..1 <br/> [Date](Date.md) |  | direct |
| [uri](uri.md) | 0..1 <br/> [uri](uri.md) |  | direct |
| [contributors](contributors.md) | * <br/> [Contribution](Contribution.md) |  | direct |
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





## Usages

| used by | used in | type | used |
| ---  | --- | --- | --- |
| [Subtask](Subtask.md) | [deliverables](deliverables.md) | range | [Deliverable](Deliverable.md) |







## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | frapo:Deliverable |
| native | sow:Deliverable |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Deliverable
description: Artifact produced by a single subtask. Subtypes specialize by category.
from_schema: https://w3id.org/collabri/sow
is_a: NamedThing
abstract: true
mixins:
- Versioned
- Trackable
attributes:
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Deliverable
    range: Contribution
    multivalued: true
    inlined: true
    inlined_as_list: true
class_uri: frapo:Deliverable

```
</details>

### Induced

<details>
```yaml
name: Deliverable
description: Artifact produced by a single subtask. Subtypes specialize by category.
from_schema: https://w3id.org/collabri/sow
is_a: NamedThing
abstract: true
mixins:
- Versioned
- Trackable
attributes:
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: category
    owner: Deliverable
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: due_date
    owner: Deliverable
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: delivered_date
    owner: Deliverable
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    alias: uri
    owner: Deliverable
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contributors
    owner: Deliverable
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
    owner: Deliverable
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
    owner: Deliverable
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
    owner: Deliverable
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Deliverable
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Deliverable
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Deliverable
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Deliverable
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
    owner: Deliverable
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
    owner: Deliverable
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
    owner: Deliverable
    domain_of:
    - NamedThing
    range: string
class_uri: frapo:Deliverable

```
</details>