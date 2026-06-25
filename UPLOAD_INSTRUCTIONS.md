# Upload Instructions

Upload these files to the QuestForge repository:

```text
README.md
.github/workflows/deploy-release.yml
```

Do not upload large game ZIP files into the repository.

Upload large builds here instead:

```text
GitHub → QuestForge repo → Releases → Draft/New release → Add files
```

Release asset filename must match:

```text
QuestForge_Current_v*.zip
```

After publishing the release:

1. Go to Settings → Pages.
2. Set Source to GitHub Actions.
3. Go to Actions.
4. Run `Deploy Latest QuestForge Release`.
5. Open the GitHub Pages link with a cache-buster, like:

```text
https://salescout2026.github.io/QuestForge/?force=v045
```
