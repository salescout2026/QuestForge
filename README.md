# QuestForge Deployment v2

This repository is intentionally small. Large playable QuestForge builds belong in GitHub Releases, not as normal repository files.

## Deployment model

1. Upload a playable ZIP to a GitHub Release.
2. The ZIP name must start with `QuestForge_Current_v` and end with `.zip`.
3. Run the `Deploy Latest QuestForge Release` workflow.
4. GitHub Pages deploys the game from that release ZIP.

Example release asset:

```text
QuestForge_Current_v045_pack_icon_linking_fix.zip
QuestForge_Current_v046_enemy_art_hotfix.zip
QuestForge_Current_v047_map_update.zip
```

The workflow automatically creates/overwrites `version.json` during deployment so the live game has one trusted version source.
