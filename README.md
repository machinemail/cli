# MachineMail CLI

`machinemail` (also installed as `mm`) is the [MachineMail](https://machinemail.dev) API from the terminal: a command for every API endpoint, plus commands built for agents and shell scripts (create an inbox, send in one line, wait for a verification code, follow new mail as it arrives). It is a single self-contained binary; you need neither Bun nor Node.

This repository only holds the release binaries. The source lives in MachineMail's main repository, which is private.

## Install

macOS and Linux (x64 and arm64, glibc):

```sh
curl -fsSL https://machinemail.dev/install.sh | sh
```

The script picks the archive for your machine from the [latest release](https://github.com/machinemail/cli/releases/latest), checks it against `SHA256SUMS`, and installs `machinemail` and `mm` into `~/.local/bin`.

Windows: download `machinemail-windows-x64.zip` from the [latest release](https://github.com/machinemail/cli/releases/latest) and unzip it into a folder on your `PATH`.

Pinned versions, completions and platform notes: [machinemail.dev/docs/cli/installation](https://machinemail.dev/docs/cli/installation).

## Releases

Tags are `cli-v<version>`. Each release has one archive per platform (`machinemail-<os>-<arch>.tar.gz`, or `.zip` on Windows), `SHA256SUMS`, and `manifest.json` with the version, commit and every asset's checksum.

## Support

Email support@machinemail.dev, or open an issue here. Include the output of `machinemail version --json`.

## License

The CLI is released under the [MIT License](LICENSE). Use of the MachineMail service is covered by the [terms of service](https://machinemail.dev/terms).
