# sync-wiki Action

Composite action at `reverberage/.github/actions/sync-wiki@main` that syncs a directory of markdown files to the repository's wiki via git push.

## Usage

```yaml
steps:
  - uses: actions/checkout@v4
    with:
      fetch-depth: 0
  - uses: reverberage/.github/actions/sync-wiki@main
    with:
      token: ${{ github.token }}
      path: docs
```

## Inputs

| Input | Required | Default | Description |
|-------|----------|---------|-------------|
| `token` | Yes | `${{ github.token }}` | GitHub token with wiki write access |
| `path` | Yes | `docs` | Directory of markdown files to sync |
| `author-name` | No | `github-actions[bot]` | Git author name |
| `author-email` | No | `41898282+github-actions[bot]@users.noreply.github.com` | Git author email |
