# ProMods Installer Unix

This repository is for the tools that will help you to install ProMods Europe on Euro Truck Simulator 2.

The current version is supporting ProMods Europe `2.61` for Euro Truck Simulator 2 `1.44.x` with addons:

* ProMods Cabin & Accessories Pack `1.18`
* ProMods Middle East `2.61`
* ProMods Trailer & Company Pack `1.32`

Please note that this repository is mainly focused on working with files, downloaded via ProMods Free Download server.

# SHA256SUMS
You can download SHA256SUMS file to just verify the checksums of the downloaded archives via `shasum -c SHA256SUMS` on macOS or `sha256sum -c SHA256SUMS` on Linux (or macOS with `coreutils` installed), if you wish to install ProMods manually.

# The ProMods Installer script
Alternatively, you can use `promods-installer-unix` script, which will verify the checksums of the downloaded archives, download 7-Zip from [7-zip.org](https://7-zip.org) (~1.5 MB of traffic), use it to extract the ProMods archives into the default mod folder location, and then clean up all temporary files it created.

This script depends on tools that are bundled in (probably most, if not all) Linux and macOS systems:


```
bash
getconf
tput
curl
tar
xz
```

To use it, download all ProMods files (with optional addons), put them into one folder and run the script in terminal from the folder with all ProMods files

For example, if all your ProMods files are located in `~/Downloads/ProMods`, and the script is located in your home folder, then you could run:
```bash
$ cd ~/Downloads/ProMods
$ ~/promods-installer-unix
```

Please also note that this script is currently in beta, so feedback in issues and/or pull requests will be appreciated.