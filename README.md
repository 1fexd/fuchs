What's this?
------------

This is a fork of Relan's excellent [fennecbuild repository](https://gitlab.com/relan/fennecbuild).
It allows compiling the entirety of Fenix without prebuilts along with removal of the proprietary blobs.

The fork adds custom patches. At this time, they are:

* Add toggle to disable the "Open in external app" prompt: [add_external_app_prompt_toggle.patch](add_external_app_prompt_toggle.patch)

This is compiled using fdroidserver.
You will need to copy the config files from -fdroiddata/ into their respective folders first.
Then run:
```
fdroid build fe.fuchs:VERCODE
```
where VERCODE is a version code number.
VERCODE is currently prepended with 2 as an epoch for upgrade from old Fennec-based Mull.
The second to last number of the VERCODE corresponds to the architecture to compile.
0 = ARMv7, 1 = x86, 2 = AArch64


Licenses
--------

Changes in the patch are licensed according to the header in the files this patch adds or modifies (Apache 2.0 or MPL 2.0).

The artwork is licensed under the MPL 2.0.

Notices
-------

Mozilla Firefox is a trademark of The Mozilla Foundation

Divested Computing Group is not affiliated with Mozilla

Mull is not sponsored or endorsed by Mozilla

Firefox source code is available at https://hg.mozilla.org
