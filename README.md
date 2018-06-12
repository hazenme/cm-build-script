# lineage-build-script
# This is a script to automate the build process and clean the out dir after each build.
# It will log the duration of the build as well as copy the .zip and .md5sum to a pre-defined folder.
# Written by Tim Clark

Place this script in your LOS source tree's base dir (eg. /android/system/)
Define the LOS_ZIP_DIR variable (nano build-lineage)

LOS_ZIP_DIR is where the .zip .md5sum and log will be moved. (Useful for syncing with Google Drive/Dropbox, etc)
This script assumes that you have Drive installed in /usr/bin/drive. (sudo apt install drive)
If you install Drive with snap, the path in the script will need to be changed to /snap/drive/22/bin/drive

Error log will be available in the LOS_ZIP_DIR as 'devicename'-log.txt (Eg. hammerhead-log.txt)

Syntax:
./build-lineage 'devicename'

Eg. ./build-lineage hammerheadcaf
