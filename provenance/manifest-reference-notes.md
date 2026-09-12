# Manifest Reference Notes — v1.0.0

Primary upstream repository: <https://github.com/OpenMW/UIX-R>

## Role of upstream manifests

The OpenMW/UIX-R manifest set is evidence used to identify historical assets, known Bethesda material and creator/source-specific groups. A manifest match is evidence; the associated permission or license context still controls.

The v1.0.0 audit used:

- `Manifests/UIXR.manifest` as the principal historical asset reference;
- `Manifests/Bethesda_IP_in_UIXR.manifest` as an exclusion/comparison reference;
- Morrowind, Tribunal and Bloodmoon comparison inventories during dependency review;
- creator/source membership recorded per row in the release-authority workbook.

The upstream manifests are linked rather than duplicated in this package. The `Master Licenses` sheet preserves source path, creator, license, manifest membership, dependencies, release decision and rights basis.

## Bethesda comparison policy

A Bethesda comparison match does not grant redistribution rights. Bethesda-owned files are not accepted into the commercial-safe authority merely because they existed in historical source material. The showcase addon instead expects the user's legally installed Morrowind runtime data where base-game resources are required.

## Temporary orphan policy

Unresolved orphan presentation assets are isolated and disclosed rather than silently assigned a license. The 400 physical files are listed in the workbook's `Orphan Disclosure` sheet and excluded from the commercial-safe claim.

## Final audit record

- Audit: project-maintainer review with Codex-assisted dependency and workbook reconciliation
- Date: 2026-09-12
- Release version: v1.0.0
- Release-authority workbook SHA-256: `c75811a9f98197b010ed2a55d45e6293e51c6ea7cc7f74cd371bc022cf96b1f2`
- Character-reference workbook SHA-256: `ea3b172d845c8869442f40b5e986f318acdfd419d19a1e42a32e213018ea2d48`
- `OpenMW_Free_Library.omwaddon` SHA-256: `4bfb2614373a5541e94f48caccfb760b6cf9613489554132c98ac17976af7a87`

