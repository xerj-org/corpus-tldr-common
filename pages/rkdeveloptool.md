# rkdeveloptool

> Flash, dump, and manage boot firmware for Rockchip-based computer devices.
> You will need to turn on the device into Maskrom/Bootrom mode before connecting it through USB.
> Some subcommands may require to run as root.
> More information: <https://github.com/rockchip-linux/rkdeveloptool>.

- list all connected Rockchip-based flash devices:

`rkdeveloptool ld`

- Initialize the device by forcing it to download and install the bootloader from the specified file:

`rkdeveloptool db {{path/to/bootloader.bin}}`

- update the bootloader software with a new one:

`rkdeveloptool ul {{path/to/bootloader.bin}}`

- Write an image to a GPT-formatted flash partition, specifying the initial storage sector (usually `0x0` alias `0`):

`rkdeveloptool wl {{initial_sector}} {{path/to/image.img}}`

- Write to the flash partition by its user-friendly name:

`rkdeveloptool wlx {{partition_name}} {{path/to/image.img}}`

- reset/reboot the device, exit from the Maskrom/Bootrom mode to boot into the selected flash partition:

`rkdeveloptool rd`
