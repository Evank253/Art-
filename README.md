# ART — Array-Associated Reverse Transcriptases

**Project status:** exploratory reconstruction and independent research notes  
**Evidence posture:** hypotheses and partial computational observations are separated from published claims and experimentally established facts.

This repository preserves the ART research project reconstructed from eight screenshots (IMG_9418–IMG_9425) and follow-up research into array-associated reverse transcriptases. ART here means **array-associated reverse transcriptases**. This repository does not claim that we have independently discovered or experimentally validated a new enzyme or biological mechanism.

## Purpose

1. Reconstruct the topic and methods described in the screenshots and related publication.
2. Separate biological mechanisms from AI-assisted discovery methods.
3. Record exploratory checks, including results that did not reproduce published coordinates.
4. Keep unresolved questions and evidence gaps visible.
5. Establish a reproducible foundation when the original screenshots, exact query artifacts, and computational environment are available.

## Current research summary

The work was prompted by Yoon et al., “Autonomous AI Agents Discover Reverse Transcriptases with Tandem Repeat Arrays.” We accessed the work through an Anthropic announcement and the alphaXiv paper/preprint view. The exact publication version, authorship metadata, supplementary files, and revisions still need verification against the primary record.

Our exploratory follow-up included a frozen 56-nucleotide query, a search against the record identified as SRR12632059_735, reverse-complement and coordinate inspection, motif/ORF review, and comparison with sequence and conserved-domain resources.

Recorded preliminary observations:
- The query's reverse complement was located at interval [154306, 154362) in the inspected sequence representation.
- The published L0050 coordinates compared during the check did not match that interval. Reference sequence, coordinate origin, strand convention, and exact publication version must be reconciled before interpreting the mismatch.
- A candidate protein of approximately 567 amino acids appeared RT-like in exploratory analysis.
- A second candidate of approximately 339 amino acids appeared RecD-family-like, but a Walker A feature was not identified in that candidate during the check.
- An approximately 8% RNA-related result was mentioned in the prior research trail, but its denominator, assay, source, and interpretation have not been independently re-established.

These are **exploratory computational observations**, not proof of a biological pathway. The exact locus, molecular interactions, functional relationship between candidates and the array, RNA result, enzymatic activity, and mechanism remain unresolved.

## Repository map

- docs/RESEARCH-DOSSIER.md — question, approach, observations, limits, evidence classification.
- docs/REPRODUCIBILITY-LOG.md — recorded analysis steps and reproduction requirements.
- docs/OPEN-QUESTIONS.md — unresolved questions and verification gates.
- references/REFERENCES.md — source trail and citation-verification checklist.
- data/README.md — data-handling rules and original-input status.

## Evidence labels

- **PUBLISHED-CLAIM** — attributed to a publication or supplement; not automatically independently verified.
- **OBSERVED-EXPLORATORY** — recorded during exploratory review; full artifacts or environment may be incomplete.
- **REPRODUCED** — independently rerun from preserved inputs with commands, versions, outputs, and hashes retained.
- **EXPERIMENTALLY-VALIDATED** — supported by appropriate experimental evidence; computational similarity alone does not qualify.
- **NOT-ESTABLISHED** — current evidence is insufficient.
- **NOT-MEASURED** — a measurement/test has not been performed or its record is unavailable.

At repository creation, no claim should be assumed REPRODUCED or EXPERIMENTALLY-VALIDATED merely because it appears in these notes.

## Scope and screenshot note

The eight original screenshots were identified as IMG_9418–IMG_9425. Their image binaries were not available in the current GitHub-writing context, so they have **not** been fabricated or represented as originals. These documents preserve the remembered research trail and flag where original screenshots and source artifacts must be reattached for faithful archival reconstruction.

## Starting points

- Anthropic news: https://www.anthropic.com/news
- alphaXiv: https://www.alphaxiv.org/
- NCBI SRA: https://www.ncbi.nlm.nih.gov/sra
- NCBI BLAST: https://blast.ncbi.nlm.nih.gov/Blast.cgi
- NCBI Conserved Domain Database: https://www.ncbi.nlm.nih.gov/Structure/cdd/cdd.shtml

See references/REFERENCES.md for source and provenance notes.
