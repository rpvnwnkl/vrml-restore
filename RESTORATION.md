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
