# cm-build-script
# This is a script to automate the build process and clean the out dir after each build.
# It will log the duration of the build as well as copy the .zip and .md5sum to a pre-defined folder.
# Written by Tim Clark

Place this script in your CM source tree's base dir (eg. /android/system/)
Edit the CM_BUILDID= and CM_ZIP_DIR= variables

CM_BUILDID will be appended to the output zip file (eg. cm-12.1-20150326-UNOFFICIAL-HAZE-hammerhead)
CM_ZIP_DIR is where the .zip .md5sum and log will be moved. (Useful for syncing with Google Drive/Dropbox, etc)

Error log will be available in the CM_ZIP_DIR as <devicename>-log.txt (Eg. hammerhead-log.txt)

Syntax:
./buildcm <devicename>

Eg. ./buildcm hammerheadcaf
