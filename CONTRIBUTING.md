# Contributing

- One new reading per PR. Run `xray publish result.json --registry . --handle NAME`.
- Commit the new reading and generated work/index changes. Run `xray registry-check .`.
- Never edit or delete existing readings. Supersede with a new reading using
  `--supersedes reading:HEX`; the old reading remains available.
- Include source identifiers, honest provenance and quotation attestations.
  Submit no source text. Readings are CC0-1.0; source quotations retain their terms.
- Maintainers review immutability and provenance; passing admission is not endorsement.

Use Node 24 and the toolchain from `camtr0n/xray-specs` at
`registry-toolchain-v1` to match CI. After cloning that tag, run `npm ci`
and `npm run build`; invoke `node /path/to/xray-specs/packages/cli/dist/main.js registry-check .`
from this registry. For an empty clone, first run `mkdir -p readings works`.
