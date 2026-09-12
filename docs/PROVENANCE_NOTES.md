# Provenance Notes — v1.0.0

The release-authority workbook is the detailed source for asset-level decisions. This document explains the model used to reach those decisions.

## Provenance chain

```text
Original creator or mod resource
        ↓
Historical use in Ultima IX: Redemption or related Morrowind resources
        ↓
OpenMW/UIX-R Libre Edition manifest, permission and licensing work
        ↓
OpenMW Free Asset Library dependency and provenance audit
        ↓
Path repair, normalization and record reconstruction
        ↓
v1.0.0 release authority
```

Not every asset passes through every step. The `Master Licenses` sheet records the evidence applicable to each authority row.

## Historical archive

Ultima IX: Redemption was a cancelled Morrowind-based fan project produced by Titans of Ether. Its publicly released archive is treated as historical source material, not as a blanket license.

Reference: <https://ultima9.ultimacodex.com/ultima-ix-redemption/>

## Upstream Libre Edition

The primary upstream authority is OpenMW/UIX-R Libre Edition: <https://github.com/OpenMW/UIX-R>

Its work includes historical asset curation, Bethesda comparison, creator contact, relicensing evidence and source-specific manifests. OpenMW Free Asset Library preserves that evidence while maintaining a separate authority for its changed paths, names, records and package layout.

## Local recovery work

The v1.0.0 process included physical-file inventory, dependency-aware record cleanup, NIF/KF and texture-path repair, asset-to-record reconstruction, public naming normalization, family/category organization, license collation and showcase CELL repair.

The final addon contains 3,003 object records, 275 CELLs and 97,740 CELL placements. Three retained public regions are Sunleaf Isle, Harborwatch Isle and Greenwarden Isle.

## Legacy names

Legacy IDs and source names remain in provenance columns when needed to trace upstream material. Public-facing names were normalized where safe. Internal IDs were retained when renaming would threaten dependency integrity.

## Temporary orphan policy

The v1.0.0 package intentionally retains 780 physical orphan/unknown files (including `_temporary_orphan` assets and unresolved legacy texture chains) for clothed example-NPC presentation and community replacement/provenance work. They are listed by path and SHA-256 in the release workbook's `Orphan Disclosure` sheet, and excluded from the commercial-safe claim.

Their status is `TEMPORARY REVIEW ONLY`. No unresolved item inherits a license from a neighboring asset.

The 141 `PLACEHOLDER_ONLY` master-authority rows are a separate reporting scope from the 780 physical orphan files.

## Authority files

- `OPENMW_FREE_ASSET_LIBRARY_RELEASE_AUTHORITY_v1.0.0.xlsx`
- `OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0.xlsx`
- `OpenMW_Free_Library.omwaddon`

The current hashes are recorded in `provenance/manifest-reference-notes.md` and `VERSION.txt`.

