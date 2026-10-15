<a href="https://tryanchor.github.io"><picture>
<source media="(prefers-color-scheme: dark)" srcset="assets/notice-dark.png">
<img src="assets/notice-light.png" alt="New: Anchor has a website. Downloads, speed tests and answers at tryanchor.github.io" width="100%">
</picture></a>

<div align="center">
<picture>
<source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png">
<img src="assets/banner-light.png" alt="Anchor: the archive tool for Windows that opens anything, extracts faster, and fixes what is broken" width="100%">
</picture>
<p>
<a href="https://github.com/realhenners/anchor-releases/releases/latest"><img src="assets/button-download.png" alt="Download for Windows" height="62"></a>&nbsp;&nbsp;<a href="https://github.com/realhenners/anchor-releases/releases"><img src="assets/button-notes.png" alt="What's new" height="62"></a>
</p>
<p><sub>Free&nbsp;&nbsp;·&nbsp;&nbsp;Windows 10 and 11&nbsp;&nbsp;·&nbsp;&nbsp;x64 and ARM64&nbsp;&nbsp;·&nbsp;&nbsp;No admin rights needed</sub></p>
<img src="assets/shot-archive.png" alt="Anchor showing the contents of a ZIP archive, with a photo preview" width="100%">
</div>

## What makes it different

<picture>
<source media="(prefers-color-scheme: dark)" srcset="assets/features-dark.png">
<img src="assets/features-light.png" alt="Open from a link. Repair any ZIP. Size map. Auto compression. Up to 2.7 times faster. Safe by default." width="100%">
</picture>

## Faster than 7-Zip and WinRAR

Anchor reads the archive as one stream and writes files in parallel. With many files that makes it up to **2.7× faster than 7-Zip** and up to **5× faster than WinRAR**, and on one 7Z archive WinRAR needed over two minutes. With large files every tool waits on decompression, so the gap is small: there Anchor stays within 0.1 s of 7-Zip (the cost of staging files so nothing is left half-written), and WinRAR is quicker on large RAR files.

<picture>
<source media="(prefers-color-scheme: dark)" srcset="assets/speed-dark.png">
<img src="assets/speed-light.png" alt="Extraction time for Anchor, 7-Zip 26.04 and WinRAR 7.23. 4,000 small files: Anchor 2.2 to 3.3 seconds, 7-Zip 5.1 to 6.5 seconds, WinRAR 3.8 seconds to over 2 minutes. A 200 MB mod pack: Anchor 0.54 to 0.69 seconds, 7-Zip 1.0 to 1.2 seconds, WinRAR 0.96 to 11.7 seconds" width="100%">
</picture>

<details>
<summary>See the numbers</summary>

| Archive | Anchor | 7-Zip 26.04 | WinRAR 7.23 |
| :-- | --: | --: | --: |
| 4,000 small files · ZIP | **2.55 s** | 5.87 s | 5.25 s |
| 4,000 small files · 7Z | **2.35 s** | 5.78 s | over 2 min |
| 4,000 small files · RAR | **2.56 s** | 5.12 s | 3.75 s |
| 4,000 small files · TAR.GZ | **2.17 s** | 5.78 s | 10.85 s |
| 4,000 small files · TAR.ZST | **3.33 s** | 6.49 s | 10.95 s |
| Mod pack: 603 files, 200 MB · ZIP | **0.61 s** | 1.02 s | 1.46 s |
| Mod pack: 603 files, 200 MB · 7Z | **0.69 s** | 1.08 s | 11.69 s |
| Mod pack: 603 files, 200 MB · RAR | **0.67 s** | 1.03 s | 0.96 s |
| Mod pack: 603 files, 200 MB · TAR.GZ | **0.54 s** | 1.20 s | 2.41 s |
| Mod pack: 603 files, 200 MB · TAR.ZST | **0.66 s** | 1.19 s | 1.81 s |
| 8 large files, 320 MB · ZIP | **0.33 s** | 0.52 s | 0.88 s |
| 8 large files, 320 MB · 7Z | 0.40 s | **0.32 s** | 0.83 s |
| 8 large files, 320 MB · RAR | 0.37 s | 0.28 s | **0.26 s** |
| 8 large files, 320 MB · TAR.GZ | **0.64 s** | 0.83 s | 1.20 s |
| 8 large files, 320 MB · TAR.ZST | **0.26 s** | 0.43 s | 0.32 s |
| 1 large file, 200 MB · ZIP | 0.41 s | **0.35 s** | 0.58 s |
| 1 large file, 200 MB · 7Z | 0.31 s | **0.24 s** | 0.34 s |
| 1 large file, 200 MB · RAR | 0.64 s | 0.57 s | **0.33 s** |
| 1 large file, 200 MB · TAR.GZ | **0.45 s** | 0.55 s | 0.76 s |
| 1 large file, 200 MB · TAR.ZST | **0.20 s** | 0.30 s | 0.24 s |

Fastest in bold. Measured on one Windows PC with 24 cores: each tool extracted every archive three times into an empty folder, producing the same files, and the best time counts. Run `npm run bench` in the source to repeat it.

</details>

## Anchor, 7-Zip and WinRAR

| | **Anchor** | 7-Zip | WinRAR |
| :-- | :--: | :--: | :--: |
| Extracts many files faster: up to 2.7× vs 7-Zip, 5× vs WinRAR | ✅ | — | — |
| Opens a ZIP from a link without downloading it all | ✅ | — | — |
| Repairs damaged ZIPs, even without recovery data | ✅ | — | ✅ |
| Recovery data for any archive | ✅ | — | RAR only |
| Size map, with duplicate files found for you | ✅ | — | — |
| Picks the right compression for your files | ✅ | — | — |
| Safety check for disguised programs and zip bombs | ✅ | — | — |
| Undo an extraction | ✅ | — | — |
| Free, with no nag screen | ✅ | ✅ | — |

## See what takes the space

The size map shows an archive by size. Click a folder to go into it. Duplicate files are found by their content, with the space they waste.

<img src="assets/shot-size-map.png" alt="Size map of an archive: folders sized by how much space they take, and a note about a duplicate file" width="100%">

## Light or dark, your choice

<img src="assets/shot-light.png" alt="Anchor in light mode, previewing a README file inside an archive" width="100%">

## Everything it does

<details>
<summary><b>Open anything</b></summary>

- Every common format, split archives from any volume, archives inside archives
- Tabs, folder tree, list and grid views, search by name or by text inside files
- Preview images, video, audio, PDF and text without extracting
- Open from a link: paste a ZIP's address (Ctrl+L) and browse it at once
- Explorer's preview pane (Alt+P) lists what is inside an archive

</details>
<details>
<summary><b>Extract safely</b></summary>

- Uses every processor core, and never puts a folder inside a folder of the same name
- Files appear only when everything succeeded, and Undo takes them back
- Checks free space first, asks before overwriting, keeps Windows' "downloaded from the internet" protection
- Right-click any archive in Explorer: Extract here, Extract to folder, Open with Anchor
- The `anchor` command in any terminal: `anchor x`, `l`, `t`, `a` and `repair`

</details>
<details>
<summary><b>Create archives</b></summary>

- ZIP, 7Z, TAR.ZST and TAR.GZ, with AES-256 passwords, split volumes and hidden file names
- Auto compression: photos and video are stored in seconds instead of crunched for minutes
- Recovery data: add 5–20% repair data so damage can be fixed later

</details>
<details>
<summary><b>Fix and check</b></summary>

- Repair from recovery data, or rebuild a broken or cut-off ZIP from whatever is still readable
- Test integrity, SHA-256 checksums, compare an archive with a folder or another archive
- Safety check flags disguised programs (`invoice.pdf.exe`), paths that escape the folder, and decompression bombs

</details>

## Install

1. Open the **[latest release](https://github.com/realhenners/anchor-releases/releases/latest)** and download `Anchor-Setup-<version>.exe`. On a Snapdragon or other ARM PC, take the file ending in `-arm64.exe`.
2. Run it and pick your options.
3. Done. Anchor checks for updates when it starts and installs them in one click.

> [!NOTE]
> **"Windows protected your PC"?** The installer is not code-signed yet, so Windows does not recognise it. Click **More info**, then **Run anyway**.

To remove Anchor: **Settings › Apps › Installed apps › Anchor › Uninstall**.

## Privacy

Anchor works offline. It goes online only to check this page for a new version when it starts (you can switch that off in Settings) and to fetch archives you open from a link. No accounts, no tracking, no telemetry.

## Help

Found a bug or have an idea? **[Open an issue](https://github.com/realhenners/anchor-releases/issues)**. A screenshot and the archive type help a lot.

## Licence

Anchor is free to use at home and at work, and closed source: © 2026 realhenners, all rights reserved. See the [licence agreement](LICENSE.txt).

<sub>Anchor includes [7-Zip](https://www.7-zip.org) (GNU LGPL), [par2cmdline](https://github.com/Parchive/par2cmdline) (GNU GPL 2.0), [Electron](https://www.electronjs.org) (MIT) and the Inter and JetBrains Mono typefaces (SIL OFL), each under its own licence. They are listed in the app under Settings › About & licences.</sub>
