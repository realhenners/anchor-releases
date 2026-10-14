<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png">
  <img src="assets/banner-light.png" alt="Anchor: the archive tool for Windows that opens anything, extracts faster, and fixes what is broken" width="100%">
</picture>

<a href="https://github.com/realhenners/anchor-releases/releases/latest"><img src="assets/button-download.png" alt="Download for Windows" width="324"></a>
<a href="https://github.com/realhenners/anchor-releases/releases"><picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/button-notes-dark.png">
  <img src="assets/button-notes-light.png" alt="What's new" width="234">
</picture></a>

<sub>Free · Windows 10 and 11 · x64 and ARM64 · No admin rights needed</sub>

<br><br>

<img src="assets/shot-archive.png" alt="Anchor showing the contents of a ZIP archive, with a photo preview" width="100%">

</div>

<br>

## What makes it different

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/features-dark.png">
  <img src="assets/features-light.png" alt="Open from a link. Repair any ZIP. Size map. Auto compression. Up to 2.6 times faster. Safe by default." width="100%">
</picture>

<br>

## Anchor, 7-Zip and WinRAR

|                                                    | **Anchor** | 7-Zip | WinRAR |
| :------------------------------------------------- | :--------: | :---: | :----: |
| Extracts many small files 2–2.6× faster            | ✅ | — | — |
| Opens a ZIP from a link without downloading it all | ✅ | — | — |
| Repairs damaged ZIPs, even without recovery data   | ✅ | — | ✅ |
| Recovery data for any archive                      | ✅ | — | RAR only |
| Size map, with duplicate files found for you       | ✅ | — | — |
| Picks the right compression for your files         | ✅ | — | — |
| Safety check for disguised programs and zip bombs  | ✅ | — | — |
| Undo an extraction                                 | ✅ | — | — |
| Free, with no nag screen                           | ✅ | ✅ | — |

<br>

## See what takes the space

The size map shows an archive by size. Click a folder to go into it. Duplicate files are found by their content, with the space they waste.

<img src="assets/shot-size-map.png" alt="Size map of an archive: folders sized by how much space they take, and a note about a duplicate file" width="100%">

<br>

## Light or dark, your choice

<img src="assets/shot-light.png" alt="Anchor in light mode, previewing a README file inside an archive" width="100%">

<br>

## Speed

Extraction time against 7-Zip 26.04 on the same PC, with the same files out.

| Archive                     | Anchor | 7-Zip |                 |
| :-------------------------- | -----: | ----: | :-------------- |
| 4,000 small files · ZIP     | 1.4 s  | 3.7 s | **2.6× faster** |
| 4,000 small files · TAR.ZST | 1.6 s  | 4.0 s | **2.5× faster** |
| 4,000 small files · TAR.GZ  | 1.7 s  | 3.7 s | **2.1× faster** |
| 320 MB in 8 large files     | 0.3–0.8 s | 0.3–0.7 s | about the same |

<br>

## Everything it does

<details>
<summary><b>Open anything</b></summary>
<br>

- Every common format, split archives from any volume, archives inside archives
- Tabs, folder tree, list and grid views, search by name or by text inside files
- Preview images, video, audio, PDF and text without extracting
- Open from a link: paste a ZIP's address (Ctrl+L) and browse it at once

</details>

<details>
<summary><b>Extract safely</b></summary>
<br>

- Uses every processor core, and never puts a folder inside a folder of the same name
- Files appear only when everything succeeded, and Undo takes them back
- Checks free space first, asks before overwriting, keeps Windows' "downloaded from the internet" protection
- Right-click any archive in Explorer: Extract here, Extract to folder, Open with Anchor

</details>

<details>
<summary><b>Create archives</b></summary>
<br>

- ZIP, 7Z, TAR.ZST and TAR.GZ, with AES-256 passwords, split volumes and hidden file names
- Auto compression: photos and video are stored in seconds instead of crunched for minutes
- Recovery data: add 5–20% repair data so damage can be fixed later

</details>

<details>
<summary><b>Fix and check</b></summary>
<br>

- Repair from recovery data, or rebuild a broken or cut-off ZIP from whatever is still readable
- Test integrity, SHA-256 checksums, compare an archive with a folder or another archive
- Safety check flags disguised programs (`invoice.pdf.exe`), paths that escape the folder, and decompression bombs

</details>

<br>

## Install

1. Open the **[latest release](https://github.com/realhenners/anchor-releases/releases/latest)** and download `Anchor-Setup-<version>.exe`.<br>
   On a Snapdragon or other ARM PC, take the file ending in `-arm64.exe`.
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
