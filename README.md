     ZephyrOS for Surnia
=================================


Instructions
---------------

Initializing:

First, create a folder to hold the source code: 

$	mkdir ~/zos
$	cd ~/zos

Initialize local repository:

	repo init -u git://github.com/Zephyr-OS/manifest.git -b zos6.0.1

Also add the local manifests:

    git clone https://github.com/ZephyrOS-falcon/local_manifests .repo/local_manifests

Sync up:

	repo sync -f --force-sync --no-clone-bundle -j4
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

First:

$	cd ~/zos
$	. /build.sh falcon
