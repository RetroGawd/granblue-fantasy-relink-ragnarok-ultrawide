# Granblue Fantasy: Relink — Ultrawide Fix (2.0 "Endless Ragnarok")

Adds ultrawide / super-ultrawide support (21:9, 32:9, any width) to Granblue Fantasy: Relink 2.0.
Native wide rendering, correct UI size, spanned HUD, and world markers that line up.

Unofficial 2.0 port of [Lyall's GBFRelinkFix](https://github.com/Lyall/GBFRelinkFix) (MIT).

## Install

Extract all files into your game folder (where `granblue_fantasy_relink.exe` is):

```
steamapps\common\Granblue Fantasy Relink
```

Launch the game — done.

**Steam Deck / Linux:** add this to the game's Steam launch options (match the included `.dll` name):

```
WINEDLLOVERRIDES="dinput8=n,b" %command%
```

## Notes

- ⚠️ Not thoroughly tested yet — please report anything odd.
- More updates coming over the next few days (FOV, camera, and more).
- Built for the current game version; a game update may require a new build.

Original mod by **Lyall** — this is an unofficial community port.
