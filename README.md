# Valheim 1.0.7 pack

Thunderstore Mod Manager will not keep patched plugin DLLs inside a `.r2z` file. On import it downloads the official Thunderstore copies and skips every `.dll` in the archive.

Download **[Valheim10-Pack.zip](Valheim10-Pack.zip)** (or the latest [Release](https://github.com/Ageous27/Valheim10-Pack/releases)), unzip it, and use the files inside.

## 1. Import the profile

1. Install Valheim **1.0.7** from Steam.
2. Open Thunderstore Mod Manager and select Valheim.
3. On the profile list, click **Import / Update -> From file**.
4. Select `Valheim10-Pack.r2z`.
5. Import as a new profile. Leave the name `Valheim10-Pack` unless you have to change it.
6. Wait until TMM finishes downloading. Do not click Play yet.

## 2. Copy the patched plugins

After import, run `ApplyPatches.cmd` (double-click). It is a regular Windows command script.

If you renamed the profile, run from a command prompt:

```bat
ApplyPatches.cmd "YourProfileName"
```

The script overwrites these plugin DLLs:

- AzuCraftyBoxes 1.8.15
- AzuExtendedPlayerInventory **2.4.13**
- Recycle_N_Reclaim **1.4.4**
- Hunting 1.4.3
- PlantEverything 1.20.0
- ItemDrawers, TargetPortal, MassFarming, AutomaticFermenters, Resurrection

Success looks like AzuEPI **2.4.13** and Recycle **1.4.4**. Then Play.

TargetPortal portal favorites use middle-click on the map, not right-click.