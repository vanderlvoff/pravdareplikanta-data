# Pravda Replikanta — editorial DATA

Public editorial JSON for https://repravda.com. Application code and infrastructure
are maintained separately in the private CODE repository.

- `main`: reviewed, published/approved editorial data.
- `develop`: experimental generator output; never published automatically.
- `data/latest/{engineer,business,enthusiast,children}/{ru,en,ja}.json`
- `data/archive/YYYY/MM/DD/`: dated issues and preserved revision folders.
- `data/schema/issue-v1.4.schema.json`: current external JSON contract.
- `data/images/`: reviewed historical editorial illustrations, referenced by JSON.

Four editions × three languages: 12 JSON files per complete current date.
Historical flat-language issues and schemas remain for compatibility. Schema
identifiers now refer to this public repository; legacy illustration source URLs
remain accepted so archived article bytes are unchanged.

## Editing

Submit new/corrected data to `develop`. Preserve dated archives and revisions;
do not replace published archives with experiments or merge into `main`
automatically. Publishing and deployment are separate actions in CODE.

Canonical schema:
https://raw.githubusercontent.com/vanderlvoff/pravdareplikanta-data/main/data/schema/issue-v1.4.schema.json

Development schema uses the same path on `develop`. Anonymous HTTPS cloning and
raw reads require no authentication. Writes require an authorized GitHub account.

Only intended public editorial data belongs here: no tokens, prompts, generator
scripts, application settings, private notes, or brand source artwork.

Initial import preserves the dated/revision directories from the published and
development CODE snapshots of 2026-11-03; these were byte-identical at migration.
This repository starts its own Git history. Earlier CODE histories and any former
public clones/forks are not rewritten or erased by this migration.
