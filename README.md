# ssh2https Action

This action changes the global git config to convert ssh URLs to https URLs.
This can be useful in two cases:

- you don't want to change your multi-repo manifest(repo, west, ...) to use
  https and you don't want to setup an additional github user with an ssh key
  either
- you want to setup a token which can access other repositories or even
  organizations

## Usage
```yaml
- uses: grandcentrix/actions-ssh2https@v1
  with:
    token: ${{ secrets.GITHUB_TOKEN }}
```
