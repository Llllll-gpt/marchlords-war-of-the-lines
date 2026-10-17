# Marchlords: War of the Lines

Marchlords is an offline territory strategy game built around match-based mana generation and battlefield commands. Lead the Blue Lions against the Red Banner across four regions to reclaim the shattered royal seal.

## Play

Download the repository as a ZIP and extract it fully. Open `index.html` in Edge or Chrome. Keep the `assets/` directory beside it. No installation or internet connection is required. Click **Enable sound** on the opening screen, or use **Enable and test sound** in Settings. The page reports blocked playback or missing audio instead of failing silently. If the test reports playback but you hear nothing, check whether this game tab is muted.

Runtime audio is bundled as standard MP3 data in local scripts, so music and effects do not depend on M4A decoding or local media-file requests. Sound effects use a shared audio context unlocked by a real click. Original recordings remain in `assets/` for archival use. The game tries the original recording if its audio bundle is unavailable.

The game includes Normal, Hard, Nightmare, and Endless March modes. Clear Stage 12 on any difficulty to unlock Endless March. Choose Chinese or English in Settings on either the main menu or the battlefield; the browser remembers your selection.

Progress is stored locally by your browser. Switching browsers, computers, or file locations may make an earlier save unavailable. If you already use the original single-file edition and want to keep its local progress, continue using that file at its existing location.

## Gameplay

- Match colored tiles to gain mana, deploy troops, and capture territory.
- Select individual squads or drag a selection box, then order them toward enemies, structures, or a destination tile. Orders can also be issued during tactical pause.
- Endless March features timed battles, upgrades between rounds, and base health that carries over.
- More details: [Gameplay and updates](GAMEPLAY_AND_UPDATES.txt), [Endless mode guide](ENDLESS_MODE_GUIDE.txt), and [World lore](WORLD_LORE.txt). These longer guides are currently written in Chinese; the game itself supports both languages.

## Repository contents

- `index.html` — complete HTML, CSS, and JavaScript game source with embedded artwork. Music and sound effects load from `assets/`.
- `assets/media/` — extracted images, music, and sound effects, named by content hash.
- Original image files are preserved in `assets/media/`. The embedded copies use lossless WebP for small artwork and quality-95 WebP for large painted backdrops.
- `assets/audio/` — sound effects that were already separate files.
- `assets/runtime/` — bundled MP3 copies used during play and their SHA-256 checksums.
- `app-icon.png` — game icon.
- `ASSETS-LICENSE.md` — media rights and reuse terms.

## License

The HTML, CSS, and JavaScript game code is available under the [MIT License](LICENSE). Images, music, sound effects, and the app icon are **not** covered by MIT; see [ASSETS-LICENSE.md](ASSETS-LICENSE.md).
