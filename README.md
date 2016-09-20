# BS_YOCTO-manifests

repo init -u https://github.com/yggdrasil31/BS_YOCTO-manifests -b krogoth -m rpi.xml
repo sync

MACHINE=raspberrypi3 ./setup-environment rpi3b-build

cd rpi3b-build
bitbake
