# premake-manager GitHub Action

This action installs the **premake-manager CLI** on GitHub Actions runners.
It supports **Windows**, **Linux**, and **macOS** automatically.

used version is 0.0.2

## Usage

Add the following to your workflow:

```yaml
jobs:
  build:
    runs-on: ubuntu-latest  # or windows-latest / macos-latest
    steps:
      - uses: actions/checkout@v4

      # Use the premake-manager action from this repo
      - uses: lolrobbe2/premake-actions/premake-manager@v1

      - name: Run premake-manager
        run: premake-manager-cli --version
```
