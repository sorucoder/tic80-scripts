# TIC-80 Scripts

Bash scripts for use with the linux version of TIC-80.

## General Features

- **Permits the use of arbitrary paths for TIC-80.** Trying to load or save catridges outside of the default directory within TIC80 is not possible. Arbitary relative or absolute paths to load and save cartridges and files can be used with these scripts (where applicable).
- **Use of one central configuration directory.** When TIC-80 has its `--fs` option set, it creates a `.local` directory to store (new) configuration. These scripts (where applicable) will link to the default configuration path. This can also be changed by setting the `$TIC80_START_PATH` variable to the `.local` directory you want to use.
- **Access outside of the working directory.** When enabled, TIC-80 can be enabled to access the entire filesystem. Note that custom configuration will be unavailable, as it sets the working directory to `/`.

## Scripts

- `tic80-develop`: Creates or loads a cartridges for development.
- `tic80-export`: Exports data from a cartridge.
- `tic80-play`: Immediately loads and plays a cartridge.
- `tic80-surf`: Invokes the TIC-80 builtin cartridge browser.
