# Agent Run downloads

This repository contains installer downloads and instructions. The Agent Run application source is maintained in a separate private repository and is not included here.

Download the matching installer from [Agent Run 0.1.0](https://github.com/MitchellMonaghan/agent-run-downloads/releases/tag/v0.1.0):

- [Linux amd64](https://github.com/MitchellMonaghan/agent-run-downloads/releases/download/v0.1.0/agent-run-0.1.0-linux-amd64.tar.gz)
- [Windows amd64 preview](https://github.com/MitchellMonaghan/agent-run-downloads/releases/download/v0.1.0/agent-run-0.1.0-windows-amd64.zip)

Extract the complete archive and keep its files together. Follow INSTALL.md inside the bundle. On Linux, run ./agent-run-setup. On Windows, open PowerShell in the extracted folder and run .\agent-run-setup-windows-amd64.exe. The installer pulls the public compiled Docker image automatically and guides account/project setup. No Go, Python or Node toolchain is required on the host.

Windows requires Windows 11 amd64 and Docker Desktop with Linux containers. The Windows executable is cross-built and unsigned; its complete native installation path is not yet tested. Linux has native installer evidence and the published image has passed a fresh anonymous download, compiled startup and SQLite health check.

Each release includes SHA256SUMS. Customer credentials and licenses are supplied to the installation at runtime. The core application source is excluded; required guest assets and third-party notices are included.

The same release archives can be hosted on a future website or S3 without changing the installer. The application image continues to come from docker.io/mitchellmonaghan/agent-run.
