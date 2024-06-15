# vcpkg-tool-snapcraft

Experiment for deploying vcpkg executable to https://snapcraft.io/

### References

* https://snapcraft.io/docs/snapcraft-tutorials
* https://snapcraft.io/docs/supported-plugins
* https://snapcraft.io/docs/snap-try
   * https://snapcraft.io/docs/debug-snaps
* https://forum.snapcraft.io/t/manual-review-of-all-new-snap-name-registrations/39440

## How To

### Build

```
snapcraft
file luncliff-vcpkg-tool_test_amd64.snap
```

### Test

After build,

```
snap install --dangerout luncliff-vcpkg-tool_test_amd64.snap
```

Run the apps in the snap package

```
luncliff-vcpkg-tool.vcpkg --help
luncliff-vcpkg-tool.vcpkg search zlib
```

Remove with the package name

```
snap remove luncliff-vcpkg-tool
```
