# The Raspberry Pi firmware files, without the ARM parts

The git history in this repository was generated from [upstream] by running
the following commands:

```
git filter-branch --prune-empty --subdirectory-filter boot
git filter-branch --prune-empty --index-filter 'git rm --cached --ignore-unmatch "kernel*.img"'
git filter-branch --prune-empty --index-filter 'git rm --cached --ignore-unmatch overlays'
```

[upstream]: https://github.com/raspberrypi/firmware/tree/bf5201e9682bf36370bc31d26b37fd4d84e1cfca
