# sixcoin Snap Packaging

Commands for building and uploading a sixcoin Core Snap to the Snap Store. Anyone on amd64 (x86_64), arm64 (aarch64), or i386 (i686) should be able to build it themselves with these instructions. This would pull the official sixcoin binaries from the releases page, verify them, and install them on a user's machine.

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
snapcraft register sixcoin-core
snapcraft upload \*.snap
sudo snap install sixcoin-core
```

### Usage
```
sixcoin-unofficial.cli # for sixcoin-cli
sixcoin-unofficial.d # for sixcoind
sixcoin-unofficial.qt # for sixcoin-qt
sixcoin-unofficial.test # for test_sixcoin
sixcoin-unofficial.tx # for sixcoin-tx
```

### Uninstalling
```
sudo snap remove sixcoin-unofficial
```