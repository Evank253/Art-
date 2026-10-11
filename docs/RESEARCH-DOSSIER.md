# ART Research Dossier

**Working title:** Reconstructing research on array-associated reverse transcriptases  
**Status:** exploratory research record; independent reproduction and biological validation remain incomplete  
**Primary reconstruction inputs:** eight screenshots identified as IMG_9418–IMG_9425 in the earlier conversation; image binaries are not included because they were not available at repository creation.

## 1. Research question

The project investigates research on reverse transcriptases associated with tandem repeat arrays and the workflow by which AI agents may help identify biological candidates. It has two related but distinct tracks:

1. **Biological track:** What sequence, repeat-array, protein, and RNA evidence supports the proposed relationship, and what mechanism—if any—has been established?
2. **Discovery-method track:** What steps were performed by the AI-assisted discovery system, what data and tools were used, and which findings can be independently reproduced?

Reconstructing an AI discovery workflow is not the same as independently validating the biological conclusion.

## 2. Publication trail

The prior research trail identified Yoon et al., “Autonomous AI Agents Discover Reverse Transcriptases with Tandem Repeat Arrays.” The work was accessed through an Anthropic announcement and an alphaXiv paper/preprint view.

**Citation status:** provisional. Before formal citation, verify the complete author list, publication venue, date, DOI or persistent identifier, exact version, supplementary material, and revisions directly against the publisher/preprint record. See ../references/REFERENCES.md.

The existence of a publication or its reported results should be represented as a published claim until the precise claim and underlying evidence have been checked.

## 3. Independent exploratory line of inquiry

The prior exploration recorded these steps:

1. Freeze a 56-nucleotide query so later checks would not silently change the input.
2. Inspect the record identified as SRR12632059_735.
3. Search for the query and its reverse complement.
4. Compare the observed sequence interval with coordinates reported for L0050.
5. Inspect candidate open reading frames and protein lengths.
6. Review sequence similarity and conserved-domain information for candidate proteins.
7. Separate what sequence analysis suggests from what would require RNA, biochemical, structural, or other experimental data.

The exact query sequence, reference accession/record metadata, command history, software versions, output files, and hashes need to be restored before this workflow can be called reproducible.

## 4. Recorded exploratory observations

### 4.1 Query and coordinate check

The recorded reverse-complement interval was [154306, 154362), a 56-nt interval under a zero-based, half-open coordinate convention. The prior comparison noted that the published L0050 coordinates did not match.

This discrepancy is unresolved. Possible causes to test—not assume—include:
- different reference sequence or assembly;
- different sequence record or read/contig representation;
- zero-based versus one-based coordinates;
- inclusive versus half-open interval conventions;
- strand orientation;
- sequence trimming or preprocessing;
- a mismatch in the interpretation of the published L0050 label.

Do not “fix” a coordinate mismatch by choosing whichever convention makes the results agree. Record the exact reference, strand, sequence, and coordinate conversion on both sides.

### 4.2 Candidate RT-like protein

A candidate of approximately 567 amino acids was recorded as RT-like during exploratory inspection. This is a similarity-based candidate description, not a demonstrated functional annotation. The full amino-acid sequence, ORF coordinates, alignment, conserved catalytic residues, domain calls, and comparison database/version need to be preserved to assess it.

**Current status:** OBSERVED-EXPLORATORY; enzymatic activity NOT-ESTABLISHED.

### 4.3 Candidate RecD-family-like protein

A second candidate of approximately 339 amino acids was described as RecD-family-like. A Walker A feature was not identified in the prior check. Failure to detect a motif in a preliminary inspection is not sufficient to conclude that the protein lacks ATPase activity or has a particular function. The sequence, alignment, search parameters, and domain-analysis output must be reviewed.

**Current status:** OBSERVED-EXPLORATORY; role in the proposed mechanism NOT-ESTABLISHED.

### 4.4 RNA-related result

The prior notes mention an approximately 8% RNA-related result. The underlying measurement and meaning have not been re-established. Without its source, denominator, controls, protocol, and statistical treatment, it must not be described as a validated biological effect or interpreted as causal evidence.

**Current status:** NOT-ESTABLISHED pending source recovery and verification.

## 5. What is not established

The current record does not establish:
- that the independently inspected interval is the exact published locus;
- that the two candidate proteins interact;
- that either candidate performs the proposed function in vivo;
- that the array causes, regulates, or is mechanistically coupled to reverse transcription;
- that the approximately 8% RNA-related figure is reproducible or biologically meaningful;
- that enzymatic activity has been measured;
- that exploratory sequence checks independently reproduce the paper's complete findings.

Computational homology, motif matches, ORF length, and coordinate proximity help prioritize tests, but none alone proves a molecular mechanism.

## 6. Evidence matrix

| Item | Recorded status | What is needed to upgrade confidence |
|---|---|---|
| Publication identification | PUBLISHED-CLAIM / citation provisional | Exact primary record, DOI or persistent ID, version, supplement |
| Frozen 56-nt query | Reported in prior research trail | Exact sequence, file, SHA-256 |
| SRR12632059_735 | Identifier recorded; context incomplete | Verify accession/record type and retrieve exact data |
| Reverse-complement interval | OBSERVED-EXPLORATORY | Reference hash, exact command, strand and coordinate convention |
| L0050 coordinate comparison | Mismatch reported | Source table/version and coordinate-system reconciliation |
| ~567-aa RT-like candidate | OBSERVED-EXPLORATORY | Sequence, ORF coordinates, alignments, domains, database versions |
| ~339-aa RecD-family-like candidate | OBSERVED-EXPLORATORY | Sequence, alignments, domain evidence, motif analysis |
| ~8% RNA-related result | NOT-ESTABLISHED | Original source, denominator, assay, controls, analysis |
| Protein interaction | NOT-ESTABLISHED | Direct evidence or appropriate experiments |
| Enzymatic activity | NOT-ESTABLISHED | Validated biochemical assay and controls |
| Overall mechanism | NOT-ESTABLISHED | Convergent, independently reproducible evidence |

## 7. Reproducibility standard

A result should be labeled REPRODUCED only after another run from preserved inputs records:
- exact input data and checksums;
- source accession and version;
- tool and database versions;
- complete commands or scripts;
- parameters and coordinate conventions;
- unedited raw outputs;
- expected versus observed results;
- failures and deviations.

Experimental claims require appropriate experimental evidence, not just a successful computational rerun.

## 8. Interpretation

The scientifically useful result at this stage is a bounded candidate and a set of explicit discrepancies/questions—not a declaration that the complete mechanism has been discovered. Preserve positive observations and unresolved checks, including the coordinate mismatch and the missing validation behind the RNA-related figure.
