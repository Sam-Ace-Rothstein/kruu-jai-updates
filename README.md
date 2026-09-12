# Kruu Jai — version pointer

This repository holds one file, `latest.json`, and nothing else. The Kruu Jai
desktop app reads it to find out whether a newer version has been released:

```json
{ "version": "0.1.0", "url": "https://…", "notes": "One line about the release" }
```

The app itself, its source and its course material are **not** here. The
download link points at a release on a private repository, so downloading asks
you to be signed in to GitHub with access to it.

## Releasing a new version

1. Build the disk image: `npm run dist` in `desktop/`.
2. Attach it to a new release on the app repository.
3. Raise `version` here and say in one line what changed.

Within a few minutes every running copy of the app offers the update the next
time it starts.
