# Project Nirwana

Welcome to Project Nirwana!

## Build Instructions

### 1. Initialize the Repository
Initialize your local repository using the Project Nirwana manifest. Ensure that Git LFS is enabled:

```bash
repo init -u https://github.com/ProjectNirwana/MANIFEST.git -b sixteen --git-lfs
```

### 2. Sync the Source
Sync the source code. The following command ensures an optimized, fast, and clean sync process:

```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```

### 3. Prepare the Build Environment
Source the build environment script:

```bash
source build/envsetup.sh
```

### 4. Choose your Device
Prepare the device-specific code. Select your product, release config, and build variant (e.g., `lunch aosp_cheetah-cp2a-userdebug`):

```bash
lunch product_name-release_config-build_variant
```

### 5. Build
Finally, start the build process:

```bash
m
```
