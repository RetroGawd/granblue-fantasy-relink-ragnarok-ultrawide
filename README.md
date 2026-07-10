[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/retrogodx)

# Granblue Fantasy: Relink Endless Ragnarok - Ultrawide Fix
Hey there, so I am not a developer and thought I would take on this challenge myself. After it started to come together I decided that others might benefit from my work. I will do my best to update or add features, but please understand it can take time. The best way to report bugs is on the Wide Screen Gaming Forum. I posted a link to the discord below. A big shoutout to everyone there who has been providing feedback, updates and appreciation for the effort!

https://discord.com/servers/wsgf-142072549537349632

### What does it do?

Adds ultrawide / super-ultrawide support (21:9, 32:9, any width) to Granblue Fantasy: Relink 2.0.
Native wide rendering, correct UI size, spanned HUD, and world markers that line up.

Extract all files into your game folder (where `granblue_fantasy_relink.exe` is):

```
steamapps\common\Granblue Fantasy Relink
```
YOU DON'T HAVE TO CHANGE THE RESOLUTION IN THE .INI FILE - YOU CAN LEAVE IT AT 0

Launch the game - done.

**IF you are having some trouble...**
1. In game settings set resolution to 3840x2160.
2. Restart the game

**IF you notice graphical glitches around your Quest Log...**
1. Remove all mods.
2. Run a file repair on Steam
3. Install mod again

### Core fixes — make ultrawide work (leave these on)

| Setting | Default | Description |
|---|---|---|
| `[Custom Resolution]` Enabled | `true` | Renders the game natively at your screen's resolution instead of a stretched 16:9. |
| `[Custom Resolution]` Width / Height | `0` | Force a render size. `0` uses your desktop resolution. |
| `[Custom Resolution]` ScreenEffects | `true` | Stretches full-screen effects (combat bursts, cutscene vignettes) to fill the screen. |
| `[Fix HUD]` Enabled | `true` | Keeps the HUD and menus at the correct size (otherwise they render oversized on a wide screen). |
| `[Span HUD]` Enabled | `true` | Spreads the in-game HUD toward the screen edges; menus and loading screens stay centered. |
| `[Span HUD]` AspectRatio | `0` | `0` = span to full width, `1.7778` = keep a centered 16:9 box, in between = partial. |
| `[Span HUD]` SpanAllHUD | `true` | `true` spreads the HUD to the edges; `false` keeps it in a centered 16:9 box. |
| `[Fix Aspect Ratio]` Enabled | `true` | Feeds your true aspect ratio to the camera so the world isn't stretched. |
| `[Fix FOV]` Enabled | `true` | Corrects field-of-view on screens narrower than 16:9. No effect on wide screens. |
| `[Fix Markers]` Enabled | `true` | Puts every world marker back on target — enemy health bars, lock-on, damage numbers, waypoints, boss gauges, and town speech bubbles. |

### Optional tweaks — personal preference (off / neutral by default)

| Setting | Default | Description |
|---|---|---|
| `[Gameplay FOV]` Multiplier | `1.0` | Field-of-view multiplier for gameplay and cutscenes. `1.0` = default, higher = wider. Max `2.5`. Link Attacks and other cinematics keep the game's own FOV, so they never warp. |
| `[Gameplay Camera Distance]` Multiplier | `1.0` | Pushes the camera back by scaling the game's own arm, so collision still applies (no clipping through walls). `1.3`–`1.8` is a good range. Max `2.5`. |
| `[Gameplay Camera Distance]` ZoomKeys | `true` | Live keyboard zoom: `=` or PageDown to pull out, `-` or PageUp to pull in, Home to reset. |
| `[Shadow Quality]` Enabled / Value | `false` / `4096` | Raises shadow resolution above the game's locked 2048. |
| `[Raise Framerate Cap]` Enabled / FPS | `false` / `240` | Lifts the frame cap while the game's Frame Rate option is set to 120 (30/60 are left alone). `0` = uncapped. |
| `[Level of Detail]` Multiplier | `1.0` | **Experimental.** Pushes object detail further into the distance to reduce pop-in. Range `0.1`–`10`. |
| `[Disable TAA]` Enabled | `false` | Turns off temporal anti-aliasing — sharper image, but more edge shimmer. |

## Notes

- ⚠️ Not thoroughly tested yet — please report anything odd.

Original mod by **Lyall** — this is an unofficial community port.
[Lyall's GBFRelinkFix](https://github.com/Lyall/GBFRelinkFix)
