# Enum: NarrativeDocumentType 




_Subtype of a narrative-document deliverable. Mapped to SPAR/FaBiO where possible._



URI: [sow:NarrativeDocumentType](https://w3id.org/collabri/sow/NarrativeDocumentType)

## Permissible Values

| Value | Meaning | Description |
| --- | --- | --- |
| policy | fabio:Policy |  |
| sop | None | Standard operating procedure |
| report | fabio:Report |  |
| recommendation | fabio:RecommendedPractice |  |
| publication | fabio:JournalArticle |  |
| preprint | fabio:Preprint |  |
| whitepaper | fabio:WhitePaper |  |
| progress_report | fabio:ProgressReport | Short progress-report blurb tied to milestone reporting |




## Slots

| Name | Description |
| ---  | --- |
| [narrative_type](narrative_type.md) |  |





## Identifier and Mapping Information






### Schema Source


* from schema: https://w3id.org/collabri/sow






## LinkML Source

<details>
```yaml
name: NarrativeDocumentType
description: Subtype of a narrative-document deliverable. Mapped to SPAR/FaBiO where
  possible.
from_schema: https://w3id.org/collabri/sow
rank: 1000
permissible_values:
  policy:
    text: policy
    meaning: fabio:Policy
  sop:
    text: sop
    description: Standard operating procedure.
  report:
    text: report
    meaning: fabio:Report
  recommendation:
    text: recommendation
    meaning: fabio:RecommendedPractice
  publication:
    text: publication
    meaning: fabio:JournalArticle
  preprint:
    text: preprint
    meaning: fabio:Preprint
  whitepaper:
    text: whitepaper
    meaning: fabio:WhitePaper
  progress_report:
    text: progress_report
    description: Short progress-report blurb tied to milestone reporting.
    meaning: fabio:ProgressReport

```
</details>