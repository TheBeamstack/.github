# HANDOVERS — H- records handed to this repo for its steward to dispose

Append-only, one record per handover. Only `cleared:` is ever edited, by the steward who disposes it
(TheBeamstack/diwan `docs/seats/hamadi.md`, R22).

## H-20261019-03 .github: the public repository has no licence; the owner ruled CC0 1.0 for it
- opened: 2026-10-19T14:46Z
- by: zayd
- from: Custodianship
- scope: item
- item: PR #1
- what: TheBeamstack/.github is public and unlicensed (main 3f1abeb has no LICENSE file, GitHub reports `license` null); the owner ruled CC0 for it in Custodianship D-20261019-01 (ANSWER: cc0); proposed text: beamstack-licensing's LICENSE at 9f0fac6, the CC0 1.0 Universal legal code GitHub detects as CC0-1.0; the item is PR #1, the PR that carries this record, because adding a licence is the owner's act and this lane adds no LICENSE file
- why: an unlicensed public repository grants no reuse right; CC0 is the licence beamstack-licensing itself carries, so the two read the same; the licence is added by the owner alone (Custodianship docs/INVARIANTS.md §1-2, T-021 done-when 2)
- evidence: `gh api repos/TheBeamstack/.github --jq '{visibility,license}'` → public, null; `gh api repos/TheBeamstack/.github/git/trees/3f1abebad6927c3ae6fde160134f9c173214f2f3 --jq '[.tree[].path]|join(" ")'` → `.github CODE_OF_CONDUCT.md CONTRIBUTING.md README.md SECURITY.md SUPPORT.md profile`; `gh api repos/TheBeamstack/beamstack-licensing --jq .license.spdx_id` → CC0-1.0; `gh api 'repos/TheBeamstack/beamstack-licensing/contents/LICENSE?ref=9f0fac6a3ff720e23a4abc60e413f160e562fe58' --jq '.sha, .size'` → 0e259d42c996742e9e3cba14c677129b2c1b6311, 7048
- need: route adding a LICENSE file to .github's main, holding beamstack-licensing's LICENSE text (blob 0e259d4), to the owner as an owner action
- cleared: -
