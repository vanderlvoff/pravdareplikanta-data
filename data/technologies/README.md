# Physical AI technology atlas

Editorial source for the private CODE repository's existing Python/Jinja renderer.
Working branch: develop. This content is separate from daily issues and the D1 encyclopedia.

- `index.json`: localized introduction, thematic categories and ordered canonical technology IDs.
- `articles/<id>.json`: metadata, explicit relationships, primary sources and twelve manuscripts
  (`ru/en/ja` × `engineer/business/enthusiast/children`).
- `diagrams/<diagram>/<lang>.svg`: original vector mechanisms with a static base and optional
  `.atlas-pulse` animation. No external resources or scripts.
- `../schema/technology-atlas-v1.schema.json`: article contract.
- `../schema/technology-index-v1.schema.json`: index contract.

`content_status: ready` marks editorial completeness, not owner authorization to publish.
Draft/withdrawn records and empty categories do not produce public article/category pages.
All references use canonical IDs, not title matching. `term_refs` must point to reviewed
encyclopedia IDs; definitions are never copied into these manuscripts. The reader fetches
current definitions from the existing ENCYCLOPEDIA_DB API.

Initial collection: 12 technologies, 144 manuscripts and 18 localized original SVGs.
Primary sources and technical review dates are included per technology. No experimental
metrics are invented. Reading-level labels come from the newspaper, not from this DATA set.

Adding a complete record and its ID to index.json extends the atlas without code changes.
Full contract, local preview and validation commands: CODE `docs/TECHNOLOGY_ATLAS.md`.
No automatic publication or schedule change is implied by adding this directory.
