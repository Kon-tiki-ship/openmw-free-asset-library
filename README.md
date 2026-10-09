# OpenMW Free Asset Library

**OpenMW Free Asset Library** is a 3D asset and game-data library designed to make it easier to develop independent games with OpenMW. Its sources and licensing information have been reviewed. The goal of the project is not merely to collect files from different sources, but to provide as clear an answer as possible to one of the most basic questions developers face when working with legacy assets:

> **“Can I actually use this asset in my project?”**

For this reason, the records in the library have been reviewed not only in terms of their technical content, but also in terms of source, license status, reuse conditions, and the legal or rights basis supporting each reuse decision. Rather than functioning solely as a conventional asset pack, OpenMW Free Asset Library has been developed as a **rights and provenance catalog** intended to clarify the reuse status of its assets.

## Version 2

Version 2 was comprehensively rebuilt to reduce the source and licensing uncertainties found in the previous release as much as possible. During this process, records from the base game Morrowind and its Tribunal and Bloodmoon expansions were compared with UIX-R manifests and licensing data, Ultima IX and Ultima IX Redemption sources, and other relevant project records. Cases in which the same asset appeared under different names, color variants, export formats, or related record types such as BODY and ARMO were reviewed separately and, where possible, connected to the same provenance chain.

With Version 2, assets were reorganized according to OpenMW’s own record structure, while `.omwgame` and `.omwaddon` files were divided into a more modular and user-friendly structure so developers can more easily select only the content they need. Assets whose source licenses could be clearly identified were linked to those licenses, while records lacking an explicit license entry but shown to be identical or technically equivalent variants of a licensed asset were evaluated through the corresponding source asset.

Assets for which no license entry could be found in the available source manifests were not automatically treated as free to use. Records considered generic or commonplace were reviewed individually; assets containing distinctive third-party design, original ornamentation, or unresolved rights issues were excluded from this category. The purpose of Version 2 is therefore not simply to provide more assets, but to **separate material considered reusable from material whose rights status remains insufficiently resolved**.

## Reuse Status

One of the catalog fields is `Reuse_Status`. When it contains `Permitted`, it means that, based on the source and rights review carried out for this library, the asset has been assessed as reusable within the scope of the project. However, where an asset is subject to a specific open license such as CC0, CC BY, or another license, the attribution requirements and other conditions of that license still apply. For that reason, `License`, `Reuse_Status`, `Source_License`, and `Rights_Basis` should be read together. The `Reuse_Status` field is populated for individually reviewed generic records and project-created NPC compositions; a blank entry does not replace the license information recorded in the other fields.

Some legacy assets have no identifiable open-source license entry or documented rightsholder, while the asset itself may consist of ordinary, functional, traditional, or otherwise commonplace forms. Such records were not automatically considered reusable; they were individually reviewed based on their visual and structural characteristics. Records for which no distinctive ornamentation, recognizable third-party design, or independently protectable creative expression could be identified use `Rights_Basis` = `Generic / Commonplace – No Identifiable Copyrightable Authorship`.

This classification does not mean that the project claims ownership of the legacy asset or purports to license it on behalf of an unknown rightsholder. On the contrary, these records use `Project_License` = `N/A` and `Ownership_Claim` = `None`. The project does not present them as “our assets released under CC0.” Instead, the assessment is that no identifiable, independently copyrightable third-party expression was found in the distributed asset, and that reuse is therefore considered permissible on that basis.

## NPCs and New Compositions

The library also contains NPC compositions created by selecting, combining, and organizing existing assets into new OpenMW character records. In these NPCs, equipment selection, character composition, record organization, and project-created character-specific data constitute separate project contributions. Where appropriate, those new contributions may therefore be released under **CC0 1.0**.

This CC0 status applies only to original contributions created by OpenMW Free Asset Library. The rights status of legacy helmets, cuirasses, boots, gloves, or other assets used within an NPC remains governed by the status listed in each asset’s own catalog record. In this way, the new NPC composition is kept legally distinct from the source rights of the legacy assets from which it is assembled.

## Source and Provenance Review

Version 2 was not based on a single manifest or project record. Records from Morrowind, Tribunal, Bloodmoon, UIX-R, Ultima IX, Ultima IX Redemption, and the OpenMW Example Suite were compared in order to construct as broad a provenance chain as possible. The Ultima IX Redemption archive was used as a historical project reference, while the UIX-R repository served as the primary upstream manifest and licensing reference.

Historical project reference:

<https://ultima9.ultimacodex.com/ultima-ix-redemption/>

Primary upstream manifest and licensing reference:

<https://github.com/OpenMW/UIX-R>

Because the absence of an asset from a manifest does not, by itself, mean that the asset is either free to use or unusable, source information and reuse decisions are kept as separate fields in the catalog. This is particularly important for legacy content that has circulated for years between mod teams, game projects, and asset packs, where the file itself may survive while creator, attribution, or licensing information is lost over time.

## Identical and Related Assets

In legacy game and mod archives, it is common for the same asset to reappear under different names, in different colors, with different export settings, or under different record types. During the preparation of Version 2, these relationships were reviewed wherever possible, and records determined to rely on the same underlying asset were linked to one another.

Where an asset could be shown to be identical or technically equivalent to another licensed record, that relationship is explicitly reflected in the catalog. As a result, a source asset that has a documented license and a related asset differing only by filename, color variant, or export detail are not automatically treated as wholly independent works. At the same time, visual similarity alone was not treated as sufficient evidence; records containing clearly distinct creative design were reviewed independently.

## OpenMW Record Structure and Additional Open Sources

The library has been reorganized according to OpenMW’s own record types. This structure is intended to allow developers to inspect only the categories of assets or game data they need and integrate them into their projects in a more controlled way. In Version 2, only example interior CELL records were retained in order to reduce unnecessary complexity, while exterior CELL records were removed from the package.

In particular, **LTEX records in Version 2 were expanded using licensed content sourced from 0 A.D.** These LTEX assets were not derived from legacy material of uncertain provenance; they were selected from **0 A.D.** assets distributed under known open licenses. This expands the pool of usable terrain and landscape resources for OpenMW while keeping the source and licensing chain of the newly added content explicit. Likewise, some records were included through the OpenMW Example Suite, while additional SOUND content was added from sources whose licensing status had been identified.

This distinction is important: Version 2 does not merely attempt to clean up older assets, but also fills gaps wherever possible with **open content whose source and license are known**. The LTEX records sourced from 0 A.D. are the clearest example of this approach.

## How to Read the Catalog

The following names reproduce the actual column headings in both published Excel catalogs. Their column positions vary by record type.

| Excel column | How to read it |
| --- | --- |
| `License` | The recorded license identifier or rights classification. Values include `CC0`, `CC0-1.0`, `CC-BY-SA-3.0`, `CC-BY`, `cc-by`, `cc-by-sa`, `N/A — Generic / Commonplace`, and `UNSPECIFIED`. Preserve the source's version information. |
| `Source` | The source reference and, where present, matching or propagation evidence. |
| `Source package` | The source-package reference retained for the record. |
| `License status` | The state or method of the license/provenance review, using the values listed below. |
| `Reuse_Status` | `Permitted` where an explicit reuse assessment is recorded. Other rows may leave this field blank. |
| `Rights_Basis` | For generic records: `Generic / Commonplace – No Identifiable Copyrightable Authorship`. For NPC compositions: `NPC Armor Composition / Selection, Coordination and Arrangement`. |
| `Source_License` | `None identified` for the reviewed generic records; `See linked asset records` for NPC compositions. Otherwise this field may be blank; consult `License` and `Source`. |
| `Project_License` | `N/A` for generic records; `CC0-1.0` for the original NPC-composition contribution. |
| `Ownership_Claim` | `None` for generic records; `Original NPC composition only — furkan yaşar` for NPC compositions. |
| `Review_Status` | `Individually reviewed` where an individual review is recorded. |
| `Technical warning` | Technical issues or missing links. This is separate from the rights review. |

Keeping these fields separate is particularly important for legacy assets. The absence of a source license does not automatically make an asset prohibited, just as an assessment that an asset is reusable does not mean that the project claims copyright ownership over it. The Version 2 catalog structure was designed specifically to distinguish between these two issues.

The following table explains the actual values used in the catalogs' `License status` column.

| Actual `License status` value | Meaning in this catalog |
| --- | --- |
| `KNOWN` | A license entry is recorded from the cited source. |
| `PROPAGATED` | License information was carried from a linked asset or provenance family; inspect `Source` and the record links. |
| `RESOLVED` | The package/provenance status is recorded as resolved. Read `License` for the applicable identifier; this status is not itself a license. |
| `Individually reviewed` | An individual review is recorded. Use the rights fields to distinguish generic records from original NPC compositions. |
| `NIF and texture provenance verified; texture paths modified` | The record's NIF and texture provenance was verified, and its texture paths were changed during integration. |
| `LICENSE_CONFIRMED; VERSION_UNKNOWN` | The source license is recorded as confirmed, but the source asset-package release/version was not supplied. For the 0 A.D. rows, `License` explicitly states `CC-BY-SA-3.0`; this status does not mean that the CC license version is unknown. |
| `CC0_CONFIRMED_BY_USER` | The project owner confirmed the CC0 information for the corresponding Ultima LTEX records. See the confirmation notice in `provenance/cc0/`. |
| `Metadata not found in source catalogs` | The searched catalogs did not supply license metadata for the record. Read its remaining fields; do not substitute a new status or license. |
| `NIF CC0; EAflame01–04 texture licenses UNSPECIFIED` | The model and its referenced textures have different recorded states. The model's CC0 entry does not supply a texture license. |

Blank rights or license fields are left blank where no value is recorded, including non-model LIGH records. `UNSPECIFIED` is a value in `License`, not another name for `RESOLVED`. Where `License` contains several identifiers separated by `|`, inspect the source and linked components rather than assuming that the identifiers are interchangeable choices.

## Purpose of Version 2

The purpose of OpenMW Free Asset Library is not to automatically declare all old game and mod files “free.” Its purpose is the opposite: **to distinguish material that can reasonably be reused from material that should not be used or requires further review**.

In legacy game-development ecosystems, thousands of assets can circulate for years between games, mod teams, community projects, and asset packs. During this process, the files may survive while the metadata identifying the original creator, first source, attribution requirements, or licensing conditions may disappear. As a result, many assets that remain technically usable can become practically inaccessible to developers simply because their provenance and licensing chain is unclear.

OpenMW Free Asset Library aims to reduce this uncertainty as much as possible and provide a clearer, reviewed, and more practical foundation for independent developers building games with OpenMW.

## Contributions and Corrections

Because this catalog deals with legacy content that has circulated between different projects and communities, new provenance information may emerge in the future. The catalog may be updated if verifiable information is found regarding an asset’s original creator, an earlier source file, a forgotten license document, a new manifest entry, or an incorrect asset match.

The project therefore does not claim to be a final and immutable historical record. Where new and verifiable evidence provides stronger provenance or rights information than an existing classification, correcting the affected records is considered a natural part of the project.

## Legal Note

This catalog is a good-faith rights and provenance review based on available manifests, source records, asset comparisons, and individual inspection. Classifying an asset as `Generic / Commonplace` does not constitute a transfer of rights or licensing on behalf of an unknown third party. OpenMW Free Asset Library licenses or waives rights only with respect to its own original contributions.

If new and verifiable provenance or rights information becomes available, the relevant records may be reassessed. Where an asset is subject to a specific third-party open license, the terms of that license always remain applicable.

## In Short

If you are a game developer evaluating an asset in the catalog, read `License`, `License status`, and the rights fields together. Where `Reuse_Status` is populated as `Permitted`, it records the explicit reuse assessment for that record. For NPC compositions, `Project_License` = `CC0-1.0` applies to the original composition contribution, while `Source_License` = `See linked asset records` directs you to the component assets. Where an asset is distributed under a specific open license, the conditions of that license must still be followed.

**OpenMW Free Asset Library v2**

*Legacy assets, clearer provenance, practical reuse.*

## Quick Installation

1. Once the Version 2 archive is published through GitHub Releases, download `OpenMW_Free_Asset_Library_v2.zip` and extract it into its own directory. A repository checkout contains catalogs and documentation, not the runtime package.
2. Register that `Data Files` directory in the configuration used by OpenMW and OpenMW-CS. Keep `meshes`, `textures`, `icons`, and `sound` inside it, beside the content files. Adding the directory does not by itself activate an addon.
3. For an independent-game project, select `OpenMW_Free_Asset_Library_v2_Base.omwgame` as the game file. Enable `OpenMW_Free_Asset_Library_v2_Assets.omwaddon` after it when the asset collection is needed.
4. To reuse the asset addon in another project, add its data directory and enable the addon in that project's content list. Check record-ID conflicts and dependencies before integrating it.
5. In OpenMW-CS, open the selected game file and the addon you want to inspect. The library provides development data and example interiors; it is not a finished playable game.

For configuration details, see the official [OpenMW installation and activation guide](https://openmw.readthedocs.io/en/stable/reference/modding/mod-install.html) and [OpenMW-CS files and directories guide](https://openmw.readthedocs.io/en/stable/manuals/openmw-cs/files-and-directories.html).

## Package Contents

| Location | Contents |
| --- | --- |
| `Data Files/OpenMW_Free_Asset_Library_v2_Base.omwgame` | Game-data foundation, construction records, terrain resources, lighting, scripts, and example interior cells. |
| `Data Files/OpenMW_Free_Asset_Library_v2_Assets.omwaddon` | Reusable character, body, equipment, creature, object, and related script records. |
| `Data Files/meshes`, `Data Files/textures`, `Data Files/icons`, `Data Files/sound` | Runtime resources shared by the content files. |
| `docs/OPENMW_FREE_ASSET_LIBRARY_BASE_CATALOG_v2.xlsx` | English record catalog for the Base game file. |
| `docs/OPENMW_FREE_ASSET_LIBRARY_ASSETS_CATALOG_v2.xlsx` | English record catalog for the Assets addon. |
| `LICENSES.md`, `LICENSES/`, `ATTRIBUTION.md`, `provenance/` | License guide, standard legal texts, credits, and supporting notices. |
| `VERSION.txt`, `CHECKSUMS.sha256` | Library version and file-integrity information. |

In the GitHub repository, `releases/` contains only a README; the catalogs and notices are at the repository root. Runtime content will be distributed separately through GitHub Releases. In the downloadable archive, runtime content is directly under the extracted package's `Data Files` directory. Quarantine content, backups, private workbooks, and Git metadata are not part of the download.

## Version Requirements

- **Library version:** v2, as recorded in `VERSION.txt`.
- **Runtime:** OpenMW with support for `.omwgame` and `.omwaddon` content files. The OpenMW engine is not bundled with this library.
- **Editor:** OpenMW-CS is required for record editing. Use the editor supplied with the same OpenMW distribution when possible.
- **Minimum engine version:** a specific minimum version has not yet been established by a compatibility test matrix for this release. Compatibility with every older OpenMW version is not claimed.
- **Catalog viewer:** an application capable of opening `.xlsx` files. Viewing the catalogs is separate from loading the content in OpenMW.
