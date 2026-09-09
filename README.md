# Xray registry

A public git repository of immutable argument readings. No database or API:
`readings/<hex>.json` holds submissions; `works/` and `index.json` enable discovery.
Consumers use `xray pull --registry https://raw.githubusercontent.com/camtr0n/xray-registry/main --list`
or point `--registry` at a local clone. Admission is not human verification or endorsement.

Contribute with `xray publish result.json --registry ./REGISTRY --handle YOUR_HANDLE`,
then commit the generated files and open a pull request. See CONTRIBUTING.md.

Readings are CC0-1.0. Quotations are short excerpts of the cited sources and
remain under their publishers' terms. Do not submit source text or credentials.

CI and Pages use [camtr0n/xray-specs](https://github.com/camtr0n/xray-specs)
pinned to `registry-toolchain-v1` with Node 24. Protect the default branch
and require the registry check.
