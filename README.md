# Xray registry

A public git repository of immutable argument readings. No database or API:
`readings/<hex>.json` holds submissions; `works/` and `index.json` enable discovery.
Consumers use `xray pull --registry https://raw.githubusercontent.com/OWNER/REPO/main --list`
or point `--registry` at a local clone. Admission is not human verification or endorsement.

Contribute with `xray publish result.json --registry ./REGISTRY --handle YOUR_HANDLE`,
then commit the generated files and open a pull request. See CONTRIBUTING.md.

Readings are CC0-1.0. Quotations are short excerpts of the cited sources and
remain under their publishers' terms. Do not submit source text or credentials.

Before enabling CI, publish the reviewed hosting implementation as the
`registry-hosting-v1` tag in camtr0n/xray-specs (or replace the workflow ref with
its immutable commit). Protect the default branch and require the registry check.
