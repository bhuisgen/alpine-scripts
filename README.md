# alpine-scripts

Boris HUISGEN <bhuisgen@hbis.fr>

Scripts to create Alpine Linux chroot environments.

## Usage

First install the required packages:

    $ sudo apt install binfmt-support qemu-user-static 

Create a configuration from a template for the needed architecture:

    $ cp config.dist.<ARCH> config
    $ vim config    

Setup the new chroot environment:

    $ sudo ./setup

Enter the chroot environment:

    $ cd /alpine-chroot-<ARCH>
    $ sudo ./run
