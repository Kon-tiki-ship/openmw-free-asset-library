# Release Package Layout — v1.0.0

The Git repository is itself a usable loose-file OpenMW data directory. A matching GitHub Release archive may be offered for users who do not clone repositories.

## Release archive

Recommended filename:

`OpenMW_Free_Asset_Library_v1.0.0.7z`

Expected contents:

```text
OpenMW_Free_Asset_Library_v1.0.0/
├─ OpenMW_Free_Library.omwaddon
├─ meshes/
├─ textures/
├─ icons/
├─ sound/
├─ docs/
│  ├─ OPENMW_FREE_ASSET_LIBRARY_RELEASE_AUTHORITY_v1.0.0.xlsx
│  ├─ OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0.xlsx
│  └─ PROVENANCE_NOTES.md
├─ provenance/
├─ README.md
├─ LICENSES.md
├─ ATTRIBUTION.md
├─ VERSION.txt
└─ CHECKSUMS.sha256
```

## Included material

- final `OpenMW_Free_Library.omwaddon`;
- public library NIF/KF assets and required textures;
- required icons and sounds;
- licensing, attribution and provenance documentation;
- v1.0.0 authority and character-reference workbooks;
- the disclosed `_temporary_orphan` presentation set.

The 400 temporary orphan physical files are retained intentionally so example NPC presentation remains visible. They must remain in their marked paths and remain excluded from commercial-safe claims.

## Excluded material

- historical raw UIX:R archives;
- old PASS/migration addons;
- scratch spreadsheets and QA CSVs;
- extraction folders, editor caches, thumbnails and local logs;
- undisclosed unresolved assets;
- Bethesda-owned files copied from a game installation;
- duplicate source copies not required by the release.

## Distribution format

v1.0.0 uses loose files so users can inspect individual assets, trace paths, reuse cleared files and diagnose OpenMW behavior. A BSA package is not required for this release.

The repository `.gitattributes` marks binary game and workbook formats as binary so Git does not apply text transformations.

## Validation

The release was tested with OpenMW 0.51.0. The addon loads after `Morrowind.esm`; Sunleaf Isle, Harborwatch Isle and Greenwarden Isle open and are navigable, and the object record catalog is visible in OpenMW-CS.

Do not validate with an older UIXRedemption/PASS data directory registered, because it can mask package files.

