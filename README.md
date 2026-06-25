# QuestForge

Production deployment repository for QuestForge 5E.

This repository is intentionally small. Large playable game builds and art packs belong in **GitHub Releases**, not as normal repository files.

## Current deployment model

- Repository stores workflow/configuration only.
- GitHub Releases store playable ZIP builds.
- GitHub Actions deploys the newest `QuestForge_Current_v*.zip` release asset to GitHub Pages.

## Upload rules

Do not commit large ZIP builds directly to the repo.

Upload playable builds to Releases using this naming pattern:

```text
QuestForge_Current_v045_pack_icon_linking_fix.zip
QuestForge_Current_v046_some_future_fix.zip
```

The workflow accepts extra words after the version number as long as the filename starts with:

```text
QuestForge_Current_v
```

## Asset packs

Large reusable art packs may also be uploaded as Release assets, for example:

```text
QuestForge_Inventory_Asset_Pack_v1.zip
```

Playable builds and asset packs can live in the same Release, but only `QuestForge_Current_v*.zip` is deployed as the playable site.
