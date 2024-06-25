# Notes on building

- GPG Key to use is ABC9F62C1B79B7BAA1BE84739AB539754304BF41
- Command to build:
```
flatpak-builder --gpg-sign=ABC9F62C1B79B7BAA1BE84739AB539754304BF41 --repo=$WHERE_THIS_REPO_WAS_CLONED/darktable-with-exiftool/repo --default-branch=with-exiftool --force-clean build org.darktable.Darktable.json 
```
Command to the repo:
```
flatpak build-update-repo --gpg-sign=ABC9F62C1B79B7BAA1BE84739AB539754304BF41  --generate-static-deltas --prune $WHERE_THIS_REPO_WAS_CLONED/darktable-with-exiftool/repo
```