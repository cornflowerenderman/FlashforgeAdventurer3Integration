# Flashforge Adventurer 3 support

This plugin adds support for the Flashforge Adventurer 3 3D printer to Cura.

Based on https://github.com/ronoaldo/FlashforgeFinderIntegration

# Install

## Binary releases

Download the latest .curapackage file from Releases page and drop it into Cura.
After you restart Cura, the plugin will be installed and you can select the new printer under Flashforge -> Flashforge Adventurer 3.
When saving the sliced file, make sure to save it as a .gx file.

## About the support for .gx (xgcode) files

GX files are normal g-code but with an extra binary header used
by FlashForge Finder and similar printers.

The header contains a few data used by the printer firmware, such as
a thumbnail of the objet to print, print time, temperature and other
information.

This work is based on the ChituCodeWriter from https://github.com/Spanni26/ChituCodeWriter
and the detailed reverse-engineering description of the binary header
from this issue on Github.
