# achroot

achroot is a script I wrote to automate chrooting.

## Dependencies

* Root (Only SuperSU tested.)
* Busybox
* A compatible chroot directory apropriate for your architecture.

## Usage

Download the file achroot from this repo and put it somewhere onto your device.

Edit the file and change the following variables:

* `CHROOT_PART`
  - Change to be the mount path of the partition your chroot is located on, say `/data`.
* `CHROOT_DIR`
  - Change it to the directory of your chroot, like `/data/local/chroot`.
* `CHROOT_CMD`
  - Change that to be the command to run when you don't pass in another command.

Given that you are `root`, have the variables correctly set up and the chroot is valid,
run the script and shortly after doing so, you should be in your chroot now!

Congratulations!

You can also run the script with arguments, such as this: `/path/to/achroot /bin/sh -c "echo Hello World."`

# License
WTFPL. See `LICENSE.md`.
