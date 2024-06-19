Getting Started:
===============

To get started with ProjectNirwana, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To initialize your local repository, use a command like this:

```bash
repo init --depth=1 -u git@github.com:ProjectNirwana/manifest.git -b fourteen --git-lfs
```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune
```

---------------------------------------------------------------------------------------
