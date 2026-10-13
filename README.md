# Soondae

A companion tool for Dark Ages: launches your characters through its own proxy, runs the
bot (abilities, walking, farming, looting, parties, alerts), and shows everything in one
window. This repo holds the **releases**; installed copies update themselves from here.

## Install

1. Download `Soondae-<version>.zip` from the [latest release](https://github.com/SJhang/Soondae/releases/latest).
2. Windows marks a downloaded zip, so SmartScreen warns on the first start. Clear the mark
   before unpacking (PowerShell, in the folder you saved it to):

   ```powershell
   Unblock-File .\Soondae-*.zip
   ```

3. Unpack anywhere you like and start `Soondae.exe`. No installer, no admin.
4. Point it at your `Darkages.exe` on **Tool settings** if it is not found by itself.

## Coming from the old tool

Start Soondae while the old tool is running (or Browse to the old exe on
**Tool settings ▸ Old tool**): it lists what the old Settings folder holds that Soondae does
not (accounts, friends, templates, map packs, rules, presets, …) and imports what you tick.
Nothing is imported by itself and the old folder is never written.

## Updates

**Tool settings ▸ Updates** checks this repo on start and on demand, downloads the next
version, verifies its SHA-256 and swaps the files when no character is connected.

## Verify a download

Each release carries a `.sha256` beside the zip:

```powershell
(Get-FileHash .\Soondae-0.1.0.zip -Algorithm SHA256).Hash
```

The source is not published here.
