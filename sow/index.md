# Statement of Work (SOW) Schema

LinkML schema for representing a Statement of Work as a contracted unit of work, with TaskTeam as the root (scoped to a single contract), Tasks as thematic buckets, recursive Subtasks, Milestones that group subtasks and trigger contractual events (e.g. payment), and typed Deliverables. The schema carries first-class change management: every element is versioned (PROV/PAV), and structural edits flow through ChangeProposals (≈ PRs) composed of element-level Changes, signed via Approvals. Classes and slots carry IRI mappings to FRAPO, PROV-O, PAV, ORG, FOAF, DCAT, DOAP, SPAR/FaBiO, IAO, ADMS, schema.org, and a layered alignment for the contract-flavored classes: FIBO Contracts (primary), ODRL (obligations/duties), Accord Project (smart-clause future), LKIF and LegalRuleML (deontics). Concordant with all via class-level exact/close/related mappings so the LinkML surface stays light while the RDF aligns with multiple ontologies.

URI: https://w3id.org/collabri/sow

Name: sow



## Classes

| Class | Description |
| --- | --- |
| [Approval](Approval.md) | Signoff on a specific version of a SOW element |
| [Change](Change.md) | Single element-level edit within a ChangeProposal |
| [ChangeProposal](ChangeProposal.md) | A bundled set of element-level Changes against a base SOW version, analogous ... |
| [Contribution](Contribution.md) | Contributor role on a deliverable, CRediT-aligned where applicable |
| [Money](Money.md) | Monetary amount with currency |
| [NamedThing](NamedThing.md) | Base class for any addressable SOW element |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Deliverable](Deliverable.md) | Artifact produced by a single subtask |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Activity](Activity.md) | An event-type deliverable (training, workshop, presentation) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Data](Data.md) | Dataset, spreadsheet, or other structured-data artifact |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Method](Method.md) | A method deliverable, modeled as a prov:Plan |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[NarrativeDocument](NarrativeDocument.md) | Policy, SOP, report, recommendation, publication, progress-report blurb, etc |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Software](Software.md) |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Standard](Standard.md) | A normative or internal standard, classified by subtype (ADMS-aligned) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Milestone](Milestone.md) | A milestone is a collection of subtasks (linked via Subtask |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Organization](Organization.md) |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Person](Person.md) |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Subtask](Subtask.md) | A step toward completion of a Task |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Task](Task.md) | Thematic bucket of work, possibly spanning the full award |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[TaskTeam](TaskTeam.md) | Root of a SOW |
| [Obligation](Obligation.md) | Abstract base for any contractual duty (ODRL pattern) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Payment](Payment.md) | Payment obligation tied to milestone acceptance |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[ReportingObligation](ReportingObligation.md) | Recurring reporting duty (quarterly progress report, annual technical report,... |
| [Party](Party.md) | A role-bearing entity in the contract |
| [Trackable](Trackable.md) | Dual-axis status for any contractually-managed element |
| [Versioned](Versioned.md) | Per-element version metadata, aligned with PAV and PROV |



## Slots

| Slot | Description |
| --- | --- |
| [acceptance_criteria](acceptance_criteria.md) | Free-text or structured criteria the sponsor uses to accept |
| [achieved_date](achieved_date.md) |  |
| [action](action.md) | ODRL action term or local action label (e |
| [activity_date](activity_date.md) |  |
| [after](after.md) | Snapshot of the element after the change (null for removes) |
| [agent](agent.md) |  |
| [amount](amount.md) |  |
| [approvals](approvals.md) | Signoffs against versions of SOW elements |
| [approved_on](approved_on.md) |  |
| [approver](approver.md) |  |
| [assignee](assignee.md) | Party bound by the obligation |
| [assigner](assigner.md) | Party imposing the obligation |
| [attendee_count](attendee_count.md) |  |
| [authored_by](authored_by.md) |  |
| [award_id](award_id.md) | Sponsor award or contract identifier |
| [base_version](base_version.md) | Version of the SOW this proposal targets |
| [basis](basis.md) |  |
| [before](before.md) | Snapshot of the element before the change (null for adds) |
| [cadence](cadence.md) | Reporting cadence (e |
| [category](category.md) |  |
| [change_proposals](change_proposals.md) | Open and historical proposals against this SOW |
| [changes](changes.md) |  |
| [collabri_doc_id](collabri_doc_id.md) | Controlled-document identifier in Collabri |
| [contract_value](contract_value.md) |  |
| [contracting_parties](contracting_parties.md) | All parties to the contract with their roles |
| [contractual_status](contractual_status.md) |  |
| [contributor](contributor.md) |  |
| [contributors](contributors.md) |  |
| [created_on](created_on.md) |  |
| [currency](currency.md) |  |
| [current_version](current_version.md) | True iff this is the current accepted version of the element |
| [decision](decision.md) | For decision-type milestones (e |
| [deliverables](deliverables.md) | Deliverables produced by this subtask |
| [delivered_date](delivered_date.md) |  |
| [description](description.md) |  |
| [distribution_url](distribution_url.md) |  |
| [due_date](due_date.md) |  |
| [effective_date](effective_date.md) |  |
| [email](email.md) |  |
| [end_date](end_date.md) |  |
| [expiration_date](expiration_date.md) |  |
| [first_due](first_due.md) |  |
| [format](format.md) |  |
| [id](id.md) | Stable ID; together with version forms the element IRI |
| [kind](kind.md) |  |
| [lead](lead.md) |  |
| [location](location.md) |  |
| [members](members.md) |  |
| [merged_on](merged_on.md) |  |
| [merged_version](merged_version.md) | Resulting SOW semver after merge |
| [milestone](milestone.md) | Milestone whose acceptance gates contractual events for this subtask |
| [milestone_type](milestone_type.md) |  |
| [milestones](milestones.md) | Milestones for this SOW |
| [name](name.md) |  |
| [narrative_type](narrative_type.md) |  |
| [obligation_class](obligation_class.md) | Discriminator for the concrete Obligation subclass |
| [obligations](obligations.md) | Non-payment obligations attached at the agreement level (reporting cadence, d... |
| [orcid](orcid.md) |  |
| [party](party.md) | Party the approver is signing on behalf of |
| [payment](payment.md) | Optional payment obligation triggered by milestone acceptance |
| [payor](payor.md) |  |
| [percent_complete](percent_complete.md) | For partial-completion payable subtasks (e |
| [performance_status](performance_status.md) |  |
| [planned_amount](planned_amount.md) |  |
| [previous_version](previous_version.md) | IRI of the immediately prior version of this element |
| [prime](prime.md) | Prime contractor under this contract |
| [prime_payable](prime_payable.md) |  |
| [program_type](program_type.md) |  |
| [proposed_by](proposed_by.md) |  |
| [proposed_on](proposed_on.md) |  |
| [protocol_url](protocol_url.md) |  |
| [rationale](rationale.md) |  |
| [record_count](record_count.md) |  |
| [repository_url](repository_url.md) |  |
| [revision](revision.md) |  |
| [role](role.md) | Contract role (sponsor, prime, subcontractor, performer, etc |
| [ror_id](ror_id.md) |  |
| [section_ref](section_ref.md) | Section under change control, if scoped narrower than the full doc |
| [signed_artifact_uri](signed_artifact_uri.md) | Pointer to the executed envelope (DocuSign, etc |
| [software_license](software_license.md) |  |
| [spans_full_award](spans_full_award.md) |  |
| [sponsor](sponsor.md) |  |
| [sponsor_payable](sponsor_payable.md) |  |
| [standard_body](standard_body.md) | Organization stewarding the standard, if external |
| [standard_subtype](standard_subtype.md) |  |
| [start_date](start_date.md) |  |
| [status](status.md) |  |
| [subtasks](subtasks.md) |  |
| [target_class](target_class.md) | Class of the target (Task, Subtask, Milestone, Deliverable,  |
| [target_date](target_date.md) |  |
| [target_id](target_id.md) | ID of the element being approved |
| [target_version](target_version.md) | pav:version of the target at time of approval |
| [tasks](tasks.md) |  |
| [template_uri](template_uri.md) | Pointer to the required reporting template, if any |
| [terms_ref](terms_ref.md) | Pointer to the governing contract clause |
| [title](title.md) |  |
| [uri](uri.md) |  |
| [version](version.md) | Semantic version of this element |
| [version_label](version_label.md) |  |


## Enumerations

| Enumeration | Description |
| --- | --- |
| [ChangeKind](ChangeKind.md) | Kind of element-level edit within a ChangeProposal |
| [ChangeProposalStatus](ChangeProposalStatus.md) | Lifecycle of a change proposal (≈ GitHub PR) |
| [ContractualStatus](ContractualStatus.md) | Where this element sits in the contract lifecycle |
| [DeliverableCategory](DeliverableCategory.md) | High-level kind of deliverable artifact |
| [MilestoneType](MilestoneType.md) | Kind of milestone event |
| [NarrativeDocumentType](NarrativeDocumentType.md) | Subtype of a narrative-document deliverable |
| [PaymentBasis](PaymentBasis.md) | How a milestone payment is structured |
| [PayorParty](PayorParty.md) | Which party owes the payable on milestone acceptance |
| [PerformanceStatus](PerformanceStatus.md) | Execution state, orthogonal to contractual status |
| [ProgramType](ProgramType.md) | Funding mechanism for the contract |
| [StandardSubtype](StandardSubtype.md) | Kinds of standards, aligned with ADMS where possible |


## Types

| Type | Description |
| --- | --- |
| [Boolean](Boolean.md) | A binary (true or false) value |
| [Curie](Curie.md) | a compact URI |
| [Date](Date.md) | a date (year, month and day) in an idealized calendar |
| [DateOrDatetime](DateOrDatetime.md) | Either a date or a datetime |
| [Datetime](Datetime.md) | The combination of a date and time |
| [Decimal](Decimal.md) | A real number with arbitrary precision that conforms to the xsd:decimal speci... |
| [Double](Double.md) | A real number that conforms to the xsd:double specification |
| [Float](Float.md) | A real number that conforms to the xsd:float specification |
| [Integer](Integer.md) | An integer |
| [Jsonpath](Jsonpath.md) | A string encoding a JSON Path |
| [Jsonpointer](Jsonpointer.md) | A string encoding a JSON Pointer |
| [Ncname](Ncname.md) | Prefix part of CURIE |
| [Nodeidentifier](Nodeidentifier.md) | A URI, CURIE or BNODE that represents a node in a model |
| [Objectidentifier](Objectidentifier.md) | A URI or CURIE that represents an object in the model |
| [Sparqlpath](Sparqlpath.md) | A string encoding a SPARQL Property Path |
| [String](String.md) | A character string |
| [Time](Time.md) | A time object represents a (local) time of day, independent of any particular... |
| [Uri](Uri.md) | a complete URI |
| [Uriorcurie](Uriorcurie.md) | a URI or a CURIE |


## Subsets

| Subset | Description |
| --- | --- |
