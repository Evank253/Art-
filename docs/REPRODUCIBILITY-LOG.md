# ART Reproducibility and Provenance Log

This log distinguishes remembered steps from runs reproducible from archived artifacts. Add new runs as new sections; do not rewrite prior results to make them appear stronger.

## Run ART-RECON-001 — reconstruction from prior conversation

- **Status:** recorded from prior research conversation; source artifacts incomplete
- **Date recorded:** 2026-10-11
- **Purpose:** preserve the research trail before it is lost across conversation or environment boundaries
- **Primary source trail:** Yoon et al., “Autonomous AI Agents Discover Reverse Transcriptases with Tandem Repeat Arrays”; Anthropic announcement; alphaXiv paper/preprint view
- **Input references:** screenshots IMG_9418–IMG_9425 (identified previously; binary files not committed)
- **Query:** frozen 56-nt query; literal sequence not present in this log and must be recovered
- **Record identifier:** SRR12632059_735; record type and exact context require confirmation
- **Tools:** prior notes mention Logan Search, sequence databases, and conserved-domain resources; exact versions and commands are unavailable here
- **Result recorded:** reverse complement observed at [154306, 154362); reported L0050 coordinates did not match
- **Candidate notes:** approximately 567-aa RT-like candidate; approximately 339-aa RecD-family-like candidate; Walker A feature not identified in the second candidate during exploratory check
- **Other note:** approximately 8% RNA-related result referenced, but source and interpretation unresolved
- **Outcome classification:** OBSERVED-EXPLORATORY, not a complete independent reproduction
- **Raw output location:** NOT RECOVERED
- **Input/output SHA-256:** NOT RECORDED
- **Independent reviewer:** NOT RECORDED

## Reproduction checklist

- [ ] Restore screenshots IMG_9418–IMG_9425 and compute SHA-256 for each.
- [ ] Recover the exact 56-nt query and store it as a text file; compute SHA-256.
- [ ] Confirm what SRR12632059_735 identifies and preserve accession metadata and retrieval date.
- [ ] Record the exact reference sequence/assembly and checksum.
- [ ] Re-run forward and reverse-complement searches using a declared coordinate convention.
- [ ] Document the published L0050 coordinates exactly as printed, including strand and source/version.
- [ ] Resolve or preserve the coordinate discrepancy without silently changing inputs.
- [ ] Preserve candidate nucleotide and amino-acid sequences with ORF coordinates.
- [ ] Record alignment commands, parameters, database versions, and raw results.
- [ ] Re-run domain/motif checks and preserve output, including negative results.
- [ ] Recover the source and definition of the approximately 8% RNA-related result.
- [ ] Have a second reviewer independently reproduce the computational observations.

## Re-run record template

Append a new section for each attempt.

### Run ID: ART-YYYYMMDD-NNN

- Operator:
- Date/time (UTC):
- Goal:
- Input filenames and SHA-256:
- Reference accession/version and SHA-256:
- Software and version:
- Database and release:
- Exact commands or script commit:
- Parameters and coordinate convention:
- Expected result:
- Observed result:
- Raw output paths and SHA-256:
- Deviations/errors:
- Interpretation:
- Evidence classification: PUBLISHED-CLAIM / OBSERVED-EXPLORATORY / REPRODUCED / EXPERIMENTALLY-VALIDATED / NOT-ESTABLISHED / NOT-MEASURED
- Independent reviewer:
- Reviewer result:

## Integrity rules

1. Do not replace raw outputs with summaries.
2. Keep failed runs and mismatches.
3. An absent result is not a negative biological finding; mark it NOT-MEASURED when appropriate.
4. Do not infer activity or mechanism from sequence similarity alone.
5. Do not mark a step reproduced unless another run can be tied to exact inputs and environment.
