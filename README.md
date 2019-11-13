# kicad2itead
Updated kicad2itead script. Original is here:https://github.com/doragasu/kicad2itead

This has been updated to work with KiCad output files in 2019. The naming conventions in KiCad have changed since the original script was created. It also creates a directory, "backup/" in the current directory and makes a copy of your files before renaming if possible.

This script renames KiCad Gerber files to match the filenames names required by iTead Studio (at https://itead.com). The script renames all the files it finds and compresses them into a ZIP file to upload to iTead. Both missing and present Gerber files are listed as the script runs.

## Usage

    kicad2itead project_name

`project name` is the substring common to all generated Gerber files (usually the project name in KiCad). Exmaple:

![alt text](https://raw.github.com/Inhibit/kicad2itead/master/kicad2itead-screenshot.png "Example run")

## Note
This script only works with two layer PCBs but can easily be extended for 4-layer boards (just add the corresponding fields to `ORG_FILES`, `DST_FILES` and `DESCRIPTS` variables).
