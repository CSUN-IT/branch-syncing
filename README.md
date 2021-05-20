# Branch Syncing

A simple GitHub Action that will keep two branches in sync.

## Usage

Simply specify the source branch (the authoritative branch) and the destination branch (the branch that will be updated).

```yaml
- uses: CSUN-IT/branch-syncing
  with:
    source: master
    destination: sync
```

### Parameters

- `source` - The source branch that will be authoritative branch
- `destination` - The branch that will be synced to match the `source` branch
- `token` - The token that will be used to pull and push branches to this repo; the default is `GITHUB_TOKEN`.
- `repository` - The repository where these branches will be managed; the default is repo this action is running in

## License

MIT
