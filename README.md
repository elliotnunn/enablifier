*Enablifier*: add a System Enabler to a Mac OS ROM file
=======================================================

Usage
-----

The destination file must first contain an Open Firmware bootinfo image (<https://github.com/elliotnunn/newworld-rom>). System Enabler data will be copied from the source file to the destination file's data and resource forks. This tool is *idempotent*: existing enabler data will be removed from the destination.

	enablify SOURCE-ENABLER DEST-FILE

Example:

	cp tbxi tbxi-enabler
	enablify templates/mac-os-rom-9.6.1 tbxi-enabler

Requirements
------------

-	Python 3
-	Rez and DeRez (part of Apple's Command Line Developer Tools)
