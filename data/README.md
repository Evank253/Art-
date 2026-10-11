# ART Data and Input Status

## Original reconstruction inputs

The prior conversation identified eight screenshots:
- IMG_9418
- IMG_9419
- IMG_9420
- IMG_9421
- IMG_9422
- IMG_9423
- IMG_9424
- IMG_9425

The image binaries were not available in the context used to initialize this repository. They have not been replaced with invented images or reconstructed from memory. Add the original files here when recovered, and record a SHA-256 for each.

## Planned layout

- screenshots/original/ — original screenshots, unmodified
- queries/ — exact frozen search query and metadata
- sequences/ — source sequence records with accession/version and checksums
- candidates/ — candidate nucleotide/protein sequences and ORF coordinates
- raw-results/ — unedited search, alignment, and domain-analysis outputs
- manifests/ — file manifest, checksums, and provenance metadata

Create these directories only when files are ready to be added; empty directories are not represented by Git.

## Data integrity rules

1. Preserve originals without recompression or editing.
2. Keep a separate copy for annotated/processed images.
3. Record file hashes, source, date, and any transformation.
4. Never commit credentials, access tokens, private keys, or unrelated personal data.
5. Check dataset terms and privacy/consent restrictions before committing potentially sensitive biological or human-subject data.
6. Every derived sequence or result must point back to its source and processing steps.
