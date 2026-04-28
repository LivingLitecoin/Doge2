# Dogecoin2 Snap Packaging

Commands for building and uploading a Dogecoin2 Core Snap to the Snap Store. Anyone on amd64 (x86_64), arm64 (aarch64), or i386 (i686) should be able to build it themselves with these instructions. This would pull the official Dogecoin2 binaries from the releases page, verify them, and install them on a user's machine.

## Building Locally
```
sudo apt install snapd
sudo snap install --classic snapcraft
sudo snapcraft
```

### Installing Locally
```
snap install \*.snap --devmode
```

### To Upload to the Snap Store
```
snapcraft login
snapcraft register dogecoin2-core
snapcraft upload \*.snap
sudo snap install dogecoin2-core
```

### Usage
```
dogecoin2-unofficial.cli # for dogecoin2-cli
dogecoin2-unofficial.d # for dogecoin2d
dogecoin2-unofficial.qt # for dogecoin2-qt
dogecoin2-unofficial.test # for test_dogecoin2
dogecoin2-unofficial.tx # for dogecoin2-tx
```

### Uninstalling
```
sudo snap remove dogecoin2-unofficial
```