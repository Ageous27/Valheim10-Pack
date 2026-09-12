# Valheim 1.0.12 pack

Thunderstore Mod Manager will not keep patched plugin DLLs inside a `.r2z` file. On import it downloads the official Thunderstore copies and skips every `.dll` in the archive.

Download **[Valheim10-Pack.zip](Valheim10-Pack.zip)** (or the latest [Release](https://github.com/Ageous27/Valheim10-Pack/releases)), unzip it, and use the files inside.

This pack matches the **Valheim Moded** Thunderstore profile (Valheim **1.0.12**, BepInExPack Valheim **5.4.2350**).

## 1. Import the profile

1. Install Valheim **1.0.12** from Steam.
2. Open Thunderstore Mod Manager and select Valheim.
3. On the profile list, click **Import / Update -> From file**.
4. Select `Valheim10-Pack.r2z`.
5. Import as a new profile. Leave the name `Valheim10-Pack` unless you have to change it.
6. Wait until TMM finishes downloading. Do not click Play yet.
7. Do not click **Update All**. That restores the unpatched Thunderstore DLLs.

## 2. Copy the patched plugins

After import, run `ApplyPatches.cmd` (double-click). It is a regular Windows command script.

If you renamed the profile, run from a command prompt:

```bat
ApplyPatches.cmd "YourProfileName"
```

The script overwrites these plugin DLLs:

- AzuExtendedPlayerInventory **2.4.13** (Thunderstore still lists 2.4.8)
- Recycle_N_Reclaim **1.4.4** (Thunderstore still lists 1.4.1)
- Hunting 1.4.3
- ItemDrawers QuickFix Unofficial (kg.ItemDrawers 1.4.0)
- PlantEverything 1.21.1 (`ZNetView.Everybody` const patch)
- PotalMap `ServerSync.dll` (`ZRoutedRpc.Everybody` const patch)
- NoAutoPickup 0.1.2
- Grass Tweaks 0.4.0 and Display BepInEx Info (local extras)

Success looks like AzuEPI **2.4.13** and Recycle **1.4.4**. Then Play.

Portal teleport is **PotalMap** (map-click), not TargetPortal.
