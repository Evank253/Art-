# ART Open Questions and Verification Gates

These questions remain open in the current reconstruction. They are questions, not conclusions.

## Gate 1 — Restore source materials

- [ ] Where are original screenshots IMG_9418–IMG_9425?
- [ ] What exact claims, diagrams, sequence strings, and citations appear in each screenshot?
- [ ] What is the exact paper version and supplementary material used during the original exploration?
- [ ] What exact 56-nt query was frozen, and what was its provenance?
- [ ] What does SRR12632059_735 refer to in the original workflow?

**Exit condition:** inputs are preserved, checksummed, and traceable to their sources.

## Gate 2 — Resolve the coordinate discrepancy

The recorded reverse-complement interval is [154306, 154362), while the L0050 coordinates compared during prior exploration did not match.

- [ ] Verify reference sequence identity and version.
- [ ] Verify whether each coordinate is zero-based or one-based.
- [ ] Verify whether end coordinates are inclusive or exclusive.
- [ ] Verify strand orientation and whether the published coordinates refer to a different object.
- [ ] Re-run the search with the exact frozen query.
- [ ] Record both the mismatch and its resolution, if found.

**Exit condition:** another reviewer can reproduce the coordinate comparison from preserved inputs.

## Gate 3 — Evaluate the approximately 567-aa RT-like candidate

- [ ] Recover the complete protein sequence and nucleotide coordinates.
- [ ] Preserve the ORF-calling method and parameters.
- [ ] Run documented similarity and conserved-domain analyses.
- [ ] Record conserved catalytic features and uncertainty.
- [ ] Compare the candidate to the exact candidate described in the paper, if applicable.

**Exit condition:** transparent computational annotation with raw output and explicit limits. This does not establish enzymatic activity.

## Gate 4 — Evaluate the approximately 339-aa RecD-family-like candidate

- [ ] Recover the exact sequence and coordinates.
- [ ] Preserve alignment/domain output and database versions.
- [ ] Revisit the reported absence of a Walker A feature using documented methods.
- [ ] Determine whether this candidate is relevant to the proposed locus or mechanism.

**Exit condition:** reproducible sequence/domain assessment. This does not establish ATPase function or a role in the mechanism.

## Gate 5 — Verify the RNA-related approximately 8% result

- [ ] Identify the exact source, figure/table, or raw data.
- [ ] Determine what the percentage measures and its denominator.
- [ ] Recover assay design, controls, sample sizes, and analysis.
- [ ] Recalculate from source data if possible.
- [ ] Distinguish association from causation.

**Exit condition:** the statistic has a defined meaning and traceable evidence—or remains NOT-ESTABLISHED.

## Gate 6 — Biological mechanism

- [ ] What evidence links the array and candidate RT?
- [ ] Is any protein-protein or protein-RNA interaction directly shown?
- [ ] Is reverse-transcriptase activity measured under appropriate controls?
- [ ] Is the proposed activity dependent on the repeat array?
- [ ] Which observations distinguish the proposed mechanism from alternatives?
- [ ] What independent experimental evidence exists?

**Exit condition:** do not claim a mechanism until evidence supports it. Computational reconstruction alone is insufficient.

## Gate 7 — Independent review

- [ ] A second reviewer receives frozen inputs and written commands.
- [ ] Reviewer reruns the analysis without hidden dependence on the first run's intermediate outputs.
- [ ] Differences are documented.
- [ ] Raw output hashes are compared.
- [ ] Claims are downgraded when a required step cannot be reproduced.

## Current stop conditions

Do not:
- claim that a novel enzyme or biological mechanism has been independently discovered;
- treat the coordinate discrepancy as resolved without evidence;
- interpret the approximately 8% RNA-related note as causal;
- equate AI-assisted discovery with independent scientific validation;
- discard failed searches, negative motifs, or conflicting coordinates.
