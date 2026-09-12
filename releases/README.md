# Release Package Layout — v1.0.0

The GitHub repository contains documentation and authority workbooks only. The full loose-file OpenMW data directory is distributed as the GitHub Release ZIP; cloning the repository alone does not install the addon or assets.

## Release archive

Recommended filename:

`OpenMW_Free_Asset_Library_v1.0.0.zip`

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
│  ├─ OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0_PUBLIC_CLEANED.xlsx
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

The documented orphan/support subset is retained intentionally as part of the current runtime/presentation context. Its files remain in their marked paths and are explicitly excluded from the release-approved licensing claim. Inclusion does not constitute a license grant; users should consult the release authority before independently reusing these files.

## Excluded material

- historical raw UIX:R archives;
- old PASS/migration addons;
- scratch spreadsheets and QA CSVs;
- extraction folders, editor caches, thumbnails and local logs;
- unresolved assets not documented by the release authority;
- Bethesda-owned files copied from a game installation;
- duplicate source copies not required by the release.

## Distribution format

v1.0.0 uses loose files so users can inspect individual assets, trace paths, reuse cleared files and diagnose OpenMW behavior. A BSA package is not required for this release.

The documentation repository `.gitattributes` marks workbooks as binary. Game binaries are distributed in the Release ZIP rather than tracked in Git.

## Validation

The documented local test target is OpenMW 0.51.0. The addon loads after `Morrowind.esm`; the three showcase regions were observed open and navigable, and the object record catalog is visible in OpenMW-CS. This documents the observed profile rather than certifying every possible installation.

Do not validate with an older UIXRedemption/PASS data directory registered, because it can mask package files.
