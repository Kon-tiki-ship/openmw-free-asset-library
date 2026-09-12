# Licensing Notes — v1.0.0

OpenMW Free Asset Library contains work from multiple creators. **There is no blanket asset license covering the complete package.** The controlling authority is:

`docs/OPENMW_FREE_ASSET_LIBRARY_RELEASE_AUTHORITY_v1.0.0.xlsx`

## Release-approved authority

The v1.0.0 release authority contains 4,807 accepted rows:

| License class | Authority rows | Release decision |
|---|---:|---|
| CC0 | 1,359 | Included |
| CC BY | 2,588 | Included with attribution |
| CC BY-SA | 860 | Included with attribution and share-alike compliance |
| **Release-approved total** | **4,807** | **Included** |

The release authority identifies 4,807 files approved for public release under documented CC0, CC BY, or CC BY-SA licensing evidence. CC BY-NC material is not part of this release-approved authority.

The authoritative creator, license, source path, manifest membership, dependency information and rights basis are recorded per file in the `Master Licenses` sheet.

## Temporary orphan material

The release also contains a documented orphan/support subset whose redistribution provenance remains unresolved. These files are retained for the current runtime/presentation context and are explicitly excluded from the release-approved licensing claim. Their inclusion does not constitute a license grant.

Their release status is:

- `ORPHAN / UNKNOWN`
- `TEMPORARY REVIEW ONLY`
- `EXCLUDED_FROM_COMMERCIAL_SAFE_CLAIM` (existing recorded status)

They are not release-cleared reusable assets and must not be described as part of the 4,807 release-approved files. Their current paths and SHA-256 hashes are listed in the `Orphan Disclosure` sheet. The associated character records are marked `DEV_ONLY_PROVENANCE_REVIEW` in the character reference workbook. Users should consult the release authority before independently reusing these files.

The 141 `PLACEHOLDER_ONLY` rows in the master authority are a separate authority-reporting scope. They must not be added to the 400 physical orphan-file count.

## How to reuse an asset

1. Find the asset in the release-authority workbook.
2. Confirm its current or legacy path and hash.
3. Read the recorded creator and license.
4. Follow the applicable attribution and share-alike requirements.
5. Treat `TEMPORARY REVIEW ONLY`, `PLACEHOLDER_ONLY`, missing or unresolved entries as outside the release-approved licensing claim.

Files beside one another do not automatically share a license.

## License references

- CC0 1.0: <https://creativecommons.org/publicdomain/zero/1.0/>
- CC BY 4.0: <https://creativecommons.org/licenses/by/4.0/>
- CC BY-SA 4.0: <https://creativecommons.org/licenses/by-sa/4.0/>

Where the authority records a different Creative Commons version or creator-specific permission context, that per-file authority controls.

## Project-authored material

Project-authored documentation and metadata are licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)** unless otherwise stated.

No project-specific code or Lua runtime is included in v1.0.0. Future original source code should carry its own license notice.

These terms do not relicense third-party meshes, textures, animations, sounds or other artwork.

## Morrowind and Bethesda material

The showcase addon requires a legally installed Morrowind runtime environment. The release does not grant rights to redistribute Bethesda game data. Upstream Bethesda/Morrowind comparison manifests are evidence used for filtering and dependency review; they are not licenses.

The historical archive is provenance, not a blanket license. Its public availability alone does not grant redistribution permission.

## Corrections

Licensing and provenance records are maintained in good faith. Original creators, rights holders or users with reliable source evidence should submit corrections through the repository's Issues section. A correction to creator, license or provenance data is treated as a priority release-documentation update.
