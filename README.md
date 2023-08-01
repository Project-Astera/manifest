# Project Astera #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/Project-Astera/manifest -b thundra
```

```bash

# Initialize local repository with this if you want to save some space
repo init -u https://github.com/Project-Astera/manifest -b thundra --depth=1
```

```bash

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh
```

```bash

# Choose a target
$ lunch aosp_devicecodename-userdebug

```bash

# Build the code
$ mka bacon -j$(nproc --all)
```