# Fate/Stay Night [Realta Nua] Ultimate Edition on Linux
This repository here provides help with _Fate/Stay Night [Realta Nua] Ultimate Edition_ installation on Linux.

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

## Configuration hints
- Set option `Display → Quality → High`. For better quality overall.
- Set option `Patch → Options → Prologue title menu`. If you want to have game menu in prologue. I find it useful.
- Unset option `Patch → Vita Additions → Play Vita OP in-game`. If you don't want spoilers.
- Set option `Patch → Movies → Force movie playback using mpv`. If you want to play movies in best compatible way.
  - On some systems movies played native way via `LAV filters`. To try it, remove `mpv.exe` from game folder.
  - If movies don't play either way or quality is poor, disable it with option `Patch → Movies → Skip movies in-game`.
