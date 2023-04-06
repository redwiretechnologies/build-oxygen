# build-oxygen
A package of the submodules to build custom openembedded images for the RWT Oxygen  SDR Development Kit
This is currently nuilt on th edunfell branch of OpenEmbedded

OpenEmbedded allows the creation of custom linux distributions for embedded systems. It is a collection of git repositories known as layers each of which provides recipes to build software packages as well as configuration information.

Information about the branch names is available at https://wiki.yoctoproject.org/wiki/Releases. Helpful articles about working with GNUradio and Openembedded are at: http://www.opensdr.com/categories/.


Install the Xilinx Vitis tools for the 2020.2 release

Getting Started
Clone the git repository:

$ git clone https://github.com/redwiretechnologies/build-oxygen.git

Update the submodules:

$ git submodule update --init

Initialize the build system:

$ TEMPLATECONF=`pwd`/meta-rwt-oxygen/conf/ source ./poky/oe-init-build-env ./build

Select the MACHINE to build for:

Build an image:

$ bitbake rwt-sdr-image


