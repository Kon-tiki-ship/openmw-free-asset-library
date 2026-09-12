# OpenMW Free Asset Library

> **Release:** v1.0.0 — 12 September 2026
> **Status:** Initial public release
> **Target:** OpenMW 0.51.0

**GitHub repository:** Documentation and authority workbooks only. Download the full addon and asset package from GitHub Releases; cloning this repository does not install the assets.

OpenMW Free Asset Library is a curated collection of reusable fantasy assets prepared for direct use in OpenMW. The project repairs broken dependencies, restores missing record links, normalizes public-facing names, and preserves per-file creator and license provenance.

The library provides native NIF, KF, DDS/TGA and OMWADDON resources together with three limited inspection/showcase environments where compatible assets can be examined in context.

This is not an official OpenMW project and is not endorsed by Bethesda Softworks, ZeniMax Media, Electronic Arts, Origin Systems or the former Ultima IX: Redemption team.

## Release contents

- `OpenMW_Free_Library.omwaddon` — 3,003 object records and the showcase content.
- `meshes/` — NIF models and KF animations.
- `textures/`, `icons/`, `sound/` — supporting assets.
- `docs/OPENMW_FREE_ASSET_LIBRARY_RELEASE_AUTHORITY_v1.0.0.xlsx` — controlling asset, record, licensing and release authority.
- `docs/OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0_PUBLIC_CLEANED.xlsx` — public technical reference for possible modular character-resource mapping.
- `LICENSES.md`, `ATTRIBUTION.md` and `docs/PROVENANCE_NOTES.md` — release policy and provenance documentation.
- `provenance/` — source-history and upstream-manifest notes.

The release authority identifies **4,807 files approved for public release under documented CC0, CC BY, or CC BY-SA licensing evidence**. The addon exposes **3,003 object records** and retains **three showcase regions**.

## Temporary orphan disclosure

The release also contains a documented orphan/support subset whose redistribution provenance remains unresolved. These files are retained for the current runtime/presentation context and are explicitly excluded from the release-approved licensing claim. Their inclusion does not constitute a license grant.

These files:

- are marked `ORPHAN / UNKNOWN` and `TEMPORARY REVIEW ONLY`;
- are excluded from the 4,807-file release-approved licensing claim;
- must not be represented as release-cleared reusable assets;
- are listed individually with path and SHA-256 in the `Orphan Disclosure` sheet of the release-authority workbook.

Users should consult the release authority before independently reusing these files.

## Historical source and upstream authority

Part of the recovered source material originated in the released archive of Ultima IX: Redemption, a cancelled Morrowind-based fan project by Titans of Ether. The archive is historical provenance, not a blanket license.

- Historical project reference: <https://ultima9.ultimacodex.com/ultima-ix-redemption/>
- Primary upstream manifest and licensing reference: <https://github.com/OpenMW/UIX-R>

OpenMW Free Asset Library is not a continuation, remake or game release of Ultima IX: Redemption. Public-facing world names and selected library record names were normalized, while legacy identifiers were retained where required for dependency safety or provenance tracing.

## Recovery and normalization work

The v1.0.0 package incorporates:

- dependency-aware removal of records that were both unnecessary for the retained library/showcase content and unsuitable for the public release;
- repair and normalization of mesh and texture paths;
- reconstruction of missing asset-to-record relationships;
- normalization of public-facing world names and selected library record names;
- creator/license collation and asset-level authority tracking;
- preservation of reusable fauna, character, architecture, prop and equipment families;
- cleanup of empty and irrelevant world content;
- retention and repair of three showcase regions;
- explicit separation of release-approved assets from the documented orphan/support subset.

## Runtime requirements

- OpenMW 0.51.0 is the documented test target. Newer versions have not been separately verified in this documentation.
- A legally installed copy of Morrowind is required for the showcase addon because it uses the standard Morrowind master/runtime environment.
- Load `Morrowind.esm` before `OpenMW_Free_Library.omwaddon`.

The physical library may be inspected independently, but use of individual assets remains subject to their per-file licenses.

## Installation

1. Download and extract the full ZIP from GitHub Releases.
2. Add the directory containing `OpenMW_Free_Library.omwaddon`, `meshes`, `textures`, `icons` and `sound` as an OpenMW data directory.
3. Enable `Morrowind.esm`.
4. Enable `OpenMW_Free_Library.omwaddon` after it.
5. Start OpenMW or open the addon in OpenMW-CS.

Example `openmw.cfg` entries:

```ini
data="C:\path\to\Morrowind\Data Files"
data="C:\path\to\OpenMW_Free_Library"
content=Morrowind.esm
content=OpenMW_Free_Library.omwaddon
```

Do not add an older UIXRedemption/PASS data directory above or below the release directory when validating the package; an older directory can mask missing or replaced files.

## Showcase regions

The addon retains three inspection areas:

- **Sunleaf Isle** — compact tropical island and settlement; central exterior CELL `108,96`.
- **Harborwatch Isle** — compact harbor island; central exterior CELL `102,97`.
- **Greenwarden Isle** — large castle and nature region; central exterior CELL `94,100`.

In the OpenMW console, `coe 108,96`, `coe 102,97` and `coe 94,100` can be used to center on those exterior cells. The regions are preview environments for browsing assets, not a standalone quest campaign.

## Character reference workbook

`docs/OPENMW_FREE_LIBRARY_CHARACTER_RACE_MAP_REFERENCE_v1.0.0_PUBLIC_CLEANED.xlsx` is a technical implementation reference showing how the existing OpenMW Free Asset Library can support a modular Human / Elf / Orc character interface. It is not a shipped character creator and is not a production roadmap.

## Licensing

The package does not have one blanket asset license. Each third-party asset retains the creator and license recorded in the release authority. Before reuse, locate the asset in the workbook and follow its CC0, CC BY, CC BY-SA or temporary-review status.

Project-authored documentation and metadata are licensed under CC BY 4.0 unless otherwise stated. This license does not replace or override third-party asset licenses.

See [LICENSES.md](LICENSES.md) and [ATTRIBUTION.md](ATTRIBUTION.md).

## Known limitations

- The documented orphan/support subset remains part of the current runtime/presentation context and outside the release-approved licensing claim.
- The character-race workbook describes possible compatibility routes; those routes are not implemented as a runtime menu.
- Some internal legacy IDs remain where renaming would break references.
- Cross-engine compatibility is not guaranteed; NIF/KF assets may require conversion.

## Feedback and corrections

Technical, licensing and attribution corrections are welcome through the Issues section of the repository distributing this release. Original creators and rights holders are encouraged to provide source or permission evidence for temporary orphan entries.

## Acknowledgements

- Original artists and modders listed in `ATTRIBUTION.md` and the release authority.
- Titans of Ether, for the historical Ultima IX: Redemption project.
- OpenMW/UIX-R Libre Edition contributors, for upstream manifest, Bethesda-IP filtering and documented licensing/permission work.
- OpenMW contributors, for the engine and editor ecosystem.

## Disclaimer

OpenMW is a separate open-source project. Ultima, Morrowind, The Elder Scrolls, Bethesda, ZeniMax, Electronic Arts, Origin Systems and related names belong to their respective owners. They are referenced only for compatibility, provenance and historical documentation.
