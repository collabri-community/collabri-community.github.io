

# Class: Task 


_Thematic bucket of work, possibly spanning the full award. Decomposed into Subtasks._





URI: [frapo:WorkPackage](http://purl.org/cerif/frapo/WorkPackage)





```mermaid
 classDiagram
    class Task
    click Task href "../Task/"
      Versioned <|-- Task
        click Versioned href "../Versioned/"
      Trackable <|-- Task
        click Trackable href "../Trackable/"
      NamedThing <|-- Task
        click NamedThing href "../NamedThing/"
      
      Task : authored_by
        
      Task : contractual_status
        
          
    
        
        
        Task --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Task : created_on
        
      Task : current_version
        
      Task : description
        
      Task : end_date
        
      Task : id
        
      Task : name
        
      Task : performance_status
        
          
    
        
        
        Task --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Task : previous_version
        
      Task : spans_full_award
        
      Task : start_date
        
      Task : subtasks
        
          
    
        
        
        Task --> "1..*" Subtask : subtasks
        click Subtask href "../Subtask/"
    

        
      Task : version
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * **Task** [ [Versioned](Versioned.md) [Trackable](Trackable.md)]



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [start_date](start_date.md) | 0..1 <br/> [Date](Date.md) |  | direct |
| [end_date](end_date.md) | 0..1 <br/> [Date](Date.md) |  | direct |
| [spans_full_award](spans_full_award.md) | 0..1 <br/> [Boolean](Boolean.md) |  | direct |
| [subtasks](subtasks.md) | 1..* <br/> [Subtask](Subtask.md) |  | direct |
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
| [TaskTeam](TaskTeam.md) | [tasks](tasks.md) | range | [Task](Task.md) |







## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow




## Mappings

| Mapping Type | Mapped Value |
| ---  | ---  |
| self | frapo:WorkPackage |
| native | sow:Task |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Task
description: Thematic bucket of work, possibly spanning the full award. Decomposed
  into Subtasks.
from_schema: https://w3id.org/collabri/sow
is_a: NamedThing
mixins:
- Versioned
- Trackable
attributes:
  start_date:
    name: start_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Task
    - Subtask
    range: date
  end_date:
    name: end_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Task
    - Subtask
    range: date
  spans_full_award:
    name: spans_full_award
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Task
    range: boolean
  subtasks:
    name: subtasks
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Task
    - Subtask
    range: Subtask
    required: true
    multivalued: true
    inlined: true
    inlined_as_list: true
class_uri: frapo:WorkPackage

```
</details>

### Induced

<details>
```yaml
name: Task
description: Thematic bucket of work, possibly spanning the full award. Decomposed
  into Subtasks.
from_schema: https://w3id.org/collabri/sow
is_a: NamedThing
mixins:
- Versioned
- Trackable
attributes:
  start_date:
    name: start_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: start_date
    owner: Task
    domain_of:
    - Task
    - Subtask
    range: date
  end_date:
    name: end_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: end_date
    owner: Task
    domain_of:
    - Task
    - Subtask
    range: date
  spans_full_award:
    name: spans_full_award
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: spans_full_award
    owner: Task
    domain_of:
    - Task
    range: boolean
  subtasks:
    name: subtasks
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: subtasks
    owner: Task
    domain_of:
    - Task
    - Subtask
    range: Subtask
    required: true
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
    owner: Task
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
    owner: Task
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
    owner: Task
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Task
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Task
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Task
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Task
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
    owner: Task
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
    owner: Task
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
    owner: Task
    domain_of:
    - NamedThing
    range: string
class_uri: frapo:WorkPackage

```
</details>