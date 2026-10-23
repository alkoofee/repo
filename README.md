# Alkoofee's Repo

A Cydia/Sileo repository with (most of) what you need for old iOS devices.

**Add it:** `https://alkoofee.github.io/repo/`

## Packages

AppSync Unified, AppSync for iOS 3.1 and 4.0, AppList, AppStoreFix, Auxo, iFile,
Cydia Substrate, PreferenceLoader, TLSFix, ultrasn0w and Veteris.

## Updating the repo

After adding or changing a `.deb` in `debs/`, rebuild the index (needs `dpkg-deb`, i.e. Linux/macOS with dpkg) so `Packages`,
`Packages.bz2` and `Packages.gz` match the files:

    python3 tools/make_packages.py debs .

`Packages.bz2` must always match `Packages` or Cydia will show stale data.
