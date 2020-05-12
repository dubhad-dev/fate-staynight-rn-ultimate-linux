# Fate/Stay Night [Realta Nua] Ultimate Edition on Linux
This repository here provides help with _Fate/Stay Night [Realta Nua] Ultimate Edition_ installation on Linux.

**UE version: `1.0.0-beta-2020-02-29`**

## Prerequisites
**You need to get original _"Fate/stay night [Realta Nua] for Windows"_ game beforehand!**

You can get it on `nyaa.si` tracker, for example.

You need to have six files:
- `Fate.rar`
- `Fate Crack.rar`
- `Heaven's Feel.7z`
- `Heaven's Feel Crack.rar`
- `Unlimited Blade Works.rar`
- `Unlimited Blade Works Crack.rar`

## Installation with [Lutris](https://lutris.net/)
1. Install `wine-staging` and needed dependenices according to your distribution instructions (for example, [Arch Linux](https://wiki.archlinux.org/index.php/Wine)).
2. Install `lutris`.
3. Run `lutris -i fate-stay-night-realta-nua-ultimate-edition.yml`
4. Follow the installation instructions.
   - Don't choose any patches in UE installator. Anyway they would be replaced by newer beta patches.
   - Don't change installation folders in UE installator.

## Installation with wine (for advanced users)
1. Install `wine` or `wine-staging` and needed dependenices according to your distribution instructions (for example, [Arch Linux](https://wiki.archlinux.org/index.php/Wine)).
2. You can create new _wineprefix_ **(recommended)** or just install it to your general _wineprefix_.
3. Install `winetricks d3dx9 quartz vcrun2015 win7`.
4. Unpack game archives in desired folder (for example, `Program Files`) inside your _wineprefix_. Result would look like this:
   - `Fate／stay night[Realta nua] -Fate-`
   - `Fate／stay night[Realta nua] -Heaven's Feel-`
   - `Fate／stay night[Realta nua] -Unlimited Blade Works-`
5. Download [installer](https://fate-patches.fra1.digitaloceanspaces.com/installer.zip), unpack and run in your _wineprefix_. Do not choose any patches.
6. Download [patches](https://fate-patches.fra1.digitaloceanspaces.com/Fate%20stay%20night%20Ultimate%20Edition%20v1.0.0-beta-2020-02-29.zip) and unpack to `Fate／stay night[Realta Nua] Ultimate Edition` folder.
7. If you want to try play movies natively install [LAV filters](https://github.com/Nevcairiel/LAVFilters/releases) to your _wineprefix_.
8. For playing movies via `mpv` download [mpv](https://sourceforge.net/projects/mpv-player-windows/files/stable/) (32bit version), unpack and copy `mpv.exe` to `Fate／stay night[Realta Nua] Ultimate Edition` folder.
9. You can delete three original game folders if you don't need them.

## Configuration hints
- Set option `Display → Quality → High`. For better quality overall.
- Set option `Patch → Options → Prologue title menu`. If you want to have game menu in prologue. I find it useful.
- Unset option `Patch → Vita Additions → Play Vita OP in-game`. If you don't want spoilers.
- Set option `Patch → Movies → Force movie playback using mpv`. If you want to play movies in best compatible way.
  - On some systems movies played native way via `LAV filters`. To try it, remove `mpv.exe` from game folder.
  - If movies don't play either way or quality is poor, disable it with option `Patch → Movies → Skip movies in-game`.

## Links
- https://github.com/leycec/fsnrnue - Installation instructions for Windows as well as for Linux. My lutris script based on script at this repo.
- https://forums.nrvnqsr.com/showthread.php/8229 - Official Ultimate Edition thread. Contains useful information about game, updates, installation, bugs and solutions. Here you can get help from UE developers and report bugs.
- https://www.xerblade.com/p/fate-stay-night-walkthrough.html?m=0 - Great game walkthrough.
