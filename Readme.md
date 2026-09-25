# ZMK Firmware
#
# Setup the build.yaml for the desired board (and also add uart exposure capabilities for ZMK Studio)
# In the west.yaml specify if wanting to compile ZMK on head or specific commit
# In config/ create 2 files for the desired keyboard name (specified in ZMK main branch itself) - .conf (where special flags reside) and .keymap (where the default keymap resides), both with the board name (needs to match 1 to 1)
# Once properly setup, once every commit, github actions should automatically start for each commit and either finish or fail (if there is a typo/issue).
# Once finished, click on the finished compile, download the .uf2 file, place the keyboard in bootloader mode and place the file in its directory (which opens once placed in bootloader mode)
# From there go to ZMK Studio and open the uart port (special button that needs to be setup in the default keymap otherwise it will not work)
# From there you can adjust each key in the keymap without needing to adjust it in the .keymap file
# 
# FYI : ZMK 4.* + is required for security type connections.
# FYI2: Security connection is required in newest bluez driver for Linux!
