# SquirrelDSP

A simple retrace of BelkaDSP schematic and board in KiCAD v7.

# Differences

- Added a few additional filtering capacitors as per ADAU1761 datasheet (they are absent in the original).
- Replaced BNC antenna connector with SMA
- Replaced USB-MicroB with USB-C connector
- SDA and SCL lines on the original PCB have 1k 1% resistors absent in the schematics, I've added them as well.
- For the LCD connector, I've chosen the first one that was suitable in terms of the number (not size!) of pins and physical dimensions.
  You should replace it with the one that suits you.

# A few words of caution

- This repo doesn't have firmware files for PIC or DSP, nor do I intend to provide them.
- There are several KiCAD errors on the PCB. Most of them are related to the SMA connector, a couple are about "bad (open) installation area" of one of the chips. If anyone wants to fix them, you're welcome.
- I've silenced KiCAD's warnings about silkscreen (there are _tons_ of them). The original board has no silkscreen at all, and it's quite difficult to fit it into such a compact size.
- Buttons positions are arbitrary; I didn’t bother with their exact positioning.

This is, first and foremost, an interesting experience of drawing somewhat complex full-fledged project in KiCAD, so I advise you to thoroughly check everything before real use.
