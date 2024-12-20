# setup-gh-cli

This action to install GitHub CLI for CodeBuild-hosted GitHub Actions runner.

## What's new

Please refer to the [release page](https://github.com/shogo452/setup-gh-cli/releases) for the latest release notes.

## Usage

```yaml
- uses: shogo452/setup-gh-cli@v1.0.7
  with:
    # Github CLI version
    # Default 2.63.2
    GH_VERSION: ''

    # Archtecture
    # Options are 'arm64' and 'amd64'.
    # Default amd64
    ARCH: ''
```

## Scenarios

### Use amd64 archtecture

```yaml
- uses: shogo452/setup-gh-cli@v1.0.7
  with:
    ARCH: arm64
```

### Use previous version

```yaml
- uses: shogo452/setup-gh-cli@v1.0.7
  with:
    GH_VERSION: 2.62.0
```
