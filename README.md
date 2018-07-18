# ChromiumOS
Outer-shell for chromiumOS

## Instructions

```
# Get repo and change into repo folder
git clone https://github.com/ChromiumOS-rPi/ChromiumOS && cd ChromiumOS

# Initialize submodule(s)
git submodule update --init --recursive

./build-environment-deps
# Setup latest stable tested revision (defaults to R56-9000.B)
./setup-revision

# The above command takes a while to finish and needs >10GB of HDD space (40-100GB per-build)
# Once complete you'll be in a chroot shell. The following command will ask you for a password 
# then spend 2-48 hours building the entire Chromium OS revision and lastly output a build image
./build_in_chroot

```

## Notes

### Chroot

Exit by typing `exit` then pressing return key (also known as enter key)

Remove by typing `cros_sdk --delete` after leaving the chroot.

