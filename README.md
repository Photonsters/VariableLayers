# VariableLayers
Variable layer files, for testing CBD-based printers/firmwares.

It seems that CBD is finally adding some support for variables layers to version 3 of the CTB file format.
[uv3dp](https://github.com/ezrec/uv3dp) has an early implementation for reading/writing these files.  Here you can find test files
that started as UVJ (created with a python script), then converted to CTB V3 with uv3dp.  The source UVJ files are
also included if you want to create a native file to test on your printer.

Not all firmwares will obey the variable layers.  The new format is made so that if the firmware does not know how to parse that info,
it will still print the file like a V2 file/firmware with a single exposure for every layer (except base layers).
