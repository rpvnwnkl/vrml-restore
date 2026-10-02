# VRML Restoration

Original VRML work circa 2002–2003.

## Preservation

The `vrml/` directory contains the surviving original project files and is
intended to remain unchanged.

The `modern/` directory contains compatibility copies for use with modern
browser-based VRML/X3D rendering.

## Alabama computer scene

`bothalabamas.wrl` assembles the monitor, computer, keyboard, and speakers.

The original scene renders successfully in X_ITE with one known compatibility
change:

- `alabama1.wrl`: the material associated with `island.jpg` used
  `diffuseColor 0.0 0.0 0.0`.
- In X_ITE this causes the loaded texture to render black.
- The modern copy changes only this material to
  `diffuseColor 1.0 1.0 1.0`, allowing the original `island.jpg`
  texture to display.

The original `vrml/alabama1.wrl` remains unchanged.

The original speaker interaction and `island.wav` audio are retained.

## Historical uncertainties

The surviving `bothalabamas.wrl` does not contain the remembered global
scene animation or background/horizon. These have not been reconstructed
because they are not present in the surviving source.

## GitHub Pages

Publish the `modern` branch from `/(root)` using Settings → Pages →
Deploy from a branch. The public site is
https://rpvnwnkl.github.io/vrml-restore/. The archival `main` branch and
`vrml/` directory are not modified by publishing. `.nojekyll` serves the
existing static viewer and assets without Jekyll processing.

The viewer keeps X_ITE pinned to 12.1.0 on jsDelivr. All scene, texture,
audio, and Inline URLs are relative, so they work beneath `/vrml-restore/`.
Audio may require a user interaction before browsers allow playback.

Pages compatibility corrections in `modern/` only:

- `computer.wrl`, `teacher.wrl`, and `teacher1.wrl` reference `Playoffs.jpg`
  with the exact capitalization of the surviving file.
- `mcdonald.wrl` references `Image3.jpg` with matching capitalization.
- The scene index omits the missing `jeepmove.wrl` and includes the surviving
  `yard.wrl`. These changes do not reconstruct missing historical content.
