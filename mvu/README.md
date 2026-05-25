# MVU Runtime Mirror

This directory mirrors the MVU runtime files used by local SillyTavern character-card scripts.

## Files

- `MagVarUpdate.bundle.js`
- `mvu_zod.js`
- `SHA256SUMS`

## Source Snapshot

- `MagVarUpdate.bundle.js`
  - Source URL: `https://testingcf.jsdelivr.net/gh/MagicalAstrogy/MagVarUpdate@master/artifact/bundle.js`
  - SHA-256: `d4c6ad5156110dac5d4e7d15d0696d1948892213e293805bb33663614d85acbb`
- `mvu_zod.js`
  - Source URL: `https://testingcf.jsdelivr.net/gh/StageDog/tavern_resource/dist/util/mvu_zod.js`
  - SHA-256: `11aceea9ec6ffdeb40bc6b417ada812087a4eb4f5817331241750960cc8d2395`

## Runtime Policy

- Character cards must import these files by pinned commit URL.
- Character cards must not import `master`, `main`, or any floating branch.
- Updating these files requires a new audit and a new pinned commit URL.

## Note

These files still contain npm CDN imports for their own dependencies. This mirror pins the entry files, not the full transitive dependency graph.
