<h2>Linux Kernel</h2>

* It is the major part of the operating system that interfaces between the computer hardware and the process. Linux Kernel is tasked with Memory Management, Process Management, Device Drivers, Syetem Calls and Security

<h3>Basic commands to understand Kernel version</h3>

* Use the `uname` command to get the type of Kernel. The `-r` i.e. `uname -r` to print the Kernel version

<h2>Working with Hardware</h2>

* The command `dmesg` is used to display message from an area of the kernel known as the ring buf     fer. Example: `dmesg | grep -i usb`. Also querying the `udev` command utility: use; `udevadm     info --query=path --name=/dev/sda5`. Also `udevadm monitor` listens to the kernel and prints     the details of events. The `lspci` commands list all the pci devices. The `lsblk` commands l     ist information about block devices. To display information about the cpu architecture, use      the `lscpu` command. The `lsmem` used to list the number of available memory in the system.      It can be used with `--summary, i.e. `lsmem --summary` to print the summary. Also, the `free    `commad can also display th   e memory and the usage. It can also be used with `-m` or `-k` e     tc display the memory in megabyte, kilobyte etc.



