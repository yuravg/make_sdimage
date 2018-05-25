make_sdimage.py
===============

Description
-----------

Just a copy of script from:
https://rocketboards.org/foswiki/Documentation/AVGSRDSdCard,
paragraph 4: Creating SD Card Image Using Provided Script.

Direct link:
http://releases.rocketboards.org/release/2018.05/gsrd/tools/make_sdimage.py

What for
--------

I am use Debian GNU/Linux 9.4 (stretch) and cannot create a file system partition FAT32.
Running the 'make_sdimage.py' script fails:

	error: format: failed

Issue
-----

By default, you are not allowed to create a filesystem across the entire device.
Set '-I' option for 'mkfs.vfat' command to work correctly.

See man 'mkfs.fat' for more information.
