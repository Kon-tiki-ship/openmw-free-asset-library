# Provenance Notes — v1.0.0

The release-authority workbook is the detailed source for asset-level decisions. This document explains the model used to reach those decisions.

## Provenance chain

```text
Original creator or mod resource
        ↓
Historical use in Ultima IX: Redemption or related Morrowind resources
        ↓
OpenMW/UIX-R Libre Edition manifest and documented permission/licensing work
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

Its work includes historical asset curation, Bethesda-IP filtering, creator/source distinction, creator contact, permission/relicensing evidence and documented Creative Commons license classes. OpenMW Free Asset Library preserves that evidence while maintaining a separate authority for its changed paths, names, records and package layout.

## Local recovery work

The v1.0.0 process included physical-file inventory, dependency-aware record cleanup, NIF/KF and texture-path repair, asset-to-record reconstruction, normalization of public-facing world names and selected library record names, family/category organization, license collation and showcase CELL repair. Legacy identifiers were retained where required for dependency safety or provenance tracing.

The final addon contains 3,003 object records, 275 CELLs and 97,740 CELL placements. Three retained public regions are Sunleaf Isle, Harborwatch Isle and Greenwarden Isle.

## Legacy names

Legacy IDs and source names remain in provenance columns when needed to trace upstream material. Public-facing names were normalized where safe. Internal IDs were retained when renaming would threaten dependency integrity.

## Temporary orphan policy

The v1.0.0 package intentionally retains a documented orphan/support subset for the current runtime/presentation context. Its files remain at their existing `_temporary_orphan` paths, are listed by path and SHA-256 in the release workbook, and are excluded from the release-approved licensing claim. Their inclusion does not constitute a license grant.

Their status is `TEMPORARY REVIEW ONLY`. No unresolved item inherits a license from a neighboring asset. Users should consult the release authority before independently reusing these files.

The 141 `PLACEHOLDER_ONLY` master-authority rows are a separate reporting scope from the 400 physical orphan files.

## Authority files

- `OPENMW_FREE_ASSET_LIBRARY_RELEASE_AUTHORITY_v1.0.0.xlsx`
- `OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0_PUBLIC_CLEANED.xlsx` (separate public documentation copy; source workbook unchanged)
- `OpenMW_Free_Library.omwaddon`

The current hashes are recorded in `provenance/manifest-reference-notes.md` and `VERSION.txt`.
