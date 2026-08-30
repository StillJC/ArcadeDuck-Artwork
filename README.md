# ArcadeDuck Artwork

Curated default artwork for ArcadeDuck's supported PS1-based arcade games.

Artwork is keyed by ArcadeDuck's canonical arcade set ID, matching the identifiers used by the ArcadeDuck game database.

## Artwork types

- clear-logo/<set-id>.png
- box-2d/<set-id>.jpg
- box-3d/<set-id>.png

Where a clone or regional variant does not have dedicated artwork, the repository materializes the selected parent artwork under the clone's own set ID. This keeps ArcadeDuck's runtime lookup intentionally simple: one direct URL per game ID, with no fuzzy title matching required.

## Runtime priority

ArcadeDuck is intended to resolve artwork in this order:

1. User-assigned/manual cover.
2. Downloaded ArcadeDuck artwork of the user's selected default type.
3. ArcadeDuck generic placeholder.

Manual artwork is never intended to be overwritten by automatic artwork downloads.

## Source

The initial curated artwork set is sourced from EmuMovies MAME artwork collections:

- MAME Game Logos Pack
- MAME 2D Boxes/Flyers Pack
- MAME (Arcade) 3D Boxes Version 2

manifest.json records whether each game uses exact artwork or a parent-inherited alias and retains the original source set ID and SHA-256.

This repository does not assign a new copyright license to third-party artwork. Artwork rights remain with their respective owners/contributors.
