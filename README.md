## TWRP device tree for Gionee M2 (WBW5506)

Add to `.repo/local_manifests/WBW5506.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/gionee/WBW5506" name="android_device_gionee_WBW5506" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_WBW5506-eng
make -j5 recoveryimage
```