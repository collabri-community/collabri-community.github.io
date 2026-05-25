

# Class: Activity 


_An event-type deliverable (training, workshop, presentation). Any associated artifact (slides, recording) is a separate deliverable._





URI: [schema:Event](http://schema.org/Event)





```mermaid
 classDiagram
    class Activity
    click Activity href "../Activity/"
      Deliverable <|-- Activity
        click Deliverable href "../Deliverable/"
      
      Activity : activity_date
        
      Activity : attendee_count
        
      Activity : authored_by
        
      Activity : category
        
          
    
        
        
        Activity --> "1" DeliverableCategory : category
        click DeliverableCategory href "../DeliverableCategory/"
    

        
      Activity : contractual_status
        
          
    
        
        
        Activity --> "1" ContractualStatus : contractual_status
        click ContractualStatus href "../ContractualStatus/"
    

        
      Activity : contributors
        
          
    
        
        
        Activity --> "*" Contribution : contributors
        click Contribution href "../Contribution/"
    

        
      Activity : created_on
        
      Activity : current_version
        
      Activity : delivered_date
        
      Activity : description
        
      Activity : due_date
        
      Activity : id
        
      Activity : location
        
      Activity : name
        
      Activity : performance_status
        
          
    
        
        
        Activity --> "0..1" PerformanceStatus : performance_status
        click PerformanceStatus href "../PerformanceStatus/"
    

        
      Activity : previous_version
        
      Activity : uri
        
      Activity : version
        
      
```





## Inheritance
* [NamedThing](NamedThing.md)
    * [Deliverable](Deliverable.md) [ [Versioned](Versioned.md) [Trackable](Trackable.md)]
        * **Activity**



## Slots

| Name | Cardinality and Range | Description | Inheritance |
| ---  | --- | --- | --- |
| [activity_date](activity_date.md) | 0..1 <br/> [Date](Date.md) |  | direct |
| [location](location.md) | 0..1 <br/> [String](String.md) |  | direct |
| [attendee_count](attendee_count.md) | 0..1 <br/> [Integer](Integer.md) |  | direct |
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
| self | schema:Event |
| native | sow:Activity |






## LinkML Source

<!-- TODO: investigate https://stackoverflow.com/questions/37606292/how-to-create-tabbed-code-blocks-in-mkdocs-or-sphinx -->

### Direct

<details>
```yaml
name: Activity
description: An event-type deliverable (training, workshop, presentation). Any associated
  artifact (slides, recording) is a separate deliverable.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(activity)
    equals_string: activity
attributes:
  activity_date:
    name: activity_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Activity
    range: date
  location:
    name: location
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: schema:location
    domain_of:
    - Activity
  attendee_count:
    name: attendee_count
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    domain_of:
    - Activity
    range: integer
class_uri: schema:Event

```
</details>

### Induced

<details>
```yaml
name: Activity
description: An event-type deliverable (training, workshop, presentation). Any associated
  artifact (slides, recording) is a separate deliverable.
from_schema: https://w3id.org/collabri/sow
is_a: Deliverable
slot_usage:
  category:
    name: category
    ifabsent: string(activity)
    equals_string: activity
attributes:
  activity_date:
    name: activity_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: activity_date
    owner: Activity
    domain_of:
    - Activity
    range: date
  location:
    name: location
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: schema:location
    alias: location
    owner: Activity
    domain_of:
    - Activity
    range: string
  attendee_count:
    name: attendee_count
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: attendee_count
    owner: Activity
    domain_of:
    - Activity
    range: integer
  category:
    name: category
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    ifabsent: string(activity)
    alias: category
    owner: Activity
    domain_of:
    - Deliverable
    range: DeliverableCategory
    required: true
    equals_string: activity
  due_date:
    name: due_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: due_date
    owner: Activity
    domain_of:
    - Deliverable
    range: date
  delivered_date:
    name: delivered_date
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: delivered_date
    owner: Activity
    domain_of:
    - Deliverable
    range: date
  uri:
    name: uri
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: dcat:landingPage
    alias: uri
    owner: Activity
    domain_of:
    - Deliverable
    range: uri
  contributors:
    name: contributors
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contributors
    owner: Activity
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
    owner: Activity
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
    owner: Activity
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
    owner: Activity
    domain_of:
    - Versioned
    range: boolean
  created_on:
    name: created_on
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:createdOn
    alias: created_on
    owner: Activity
    domain_of:
    - Versioned
    range: date
  authored_by:
    name: authored_by
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    slot_uri: pav:authoredBy
    alias: authored_by
    owner: Activity
    domain_of:
    - Versioned
    range: uriorcurie
    multivalued: true
  contractual_status:
    name: contractual_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: contractual_status
    owner: Activity
    domain_of:
    - Trackable
    range: ContractualStatus
    required: true
  performance_status:
    name: performance_status
    from_schema: https://w3id.org/collabri/sow
    rank: 1000
    alias: performance_status
    owner: Activity
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
    owner: Activity
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
    owner: Activity
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
    owner: Activity
    domain_of:
    - NamedThing
    range: string
class_uri: schema:Event

```
</details>