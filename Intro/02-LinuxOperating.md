![image](https://github.com/user-attachments/assets/e2e8d78b-e23d-42ec-84f8-a9f34671cc29)

BIOS(Basic Input and Output) initializes the screeena and keyboard and testz the main memory. This process is know as **Power-On Self-Test (POST)** is a diagnostic testing sequence performed by a computer's firmware (BIOS or UEFI) when the system is powered on.
This BIOS is in ROM(Read Only Memory)  specifically in a type of non-volatile memory.
RTC- Real Time Clock   which keeps track of the date and time in a Linux system, is powered by a small CMOS battery (often called a BIOS or motherboard battery). 

Once BIOS is completed, it is then control goes to Boot Loader. The Boot Loader is present in one of the hard-disk in the system. EIther in the boot-sector for traditional bios or **Master Boot Record(MBR)** This is know as First Sector of Hard Disk

![image](https://github.com/user-attachments/assets/fb251fb8-089b-4061-876e-f797d1599141)

The **boot loader** in Linux is a small program that loads the operating system kernel into memory and starts its execution.

BootLoader is responsible for OS and file system to load 

![image](https://github.com/user-attachments/assets/16133e7f-6b6e-4f84-ad50-dfd59828bd8b)


initramfs (Initial RAM Filesystem) is a temporary root filesystem used during the Linux boot process. It is loaded into memory by the bootloader (like GRUB) and provides the necessary tools and drivers to mount the real root filesystem.

![image](https://github.com/user-attachments/assets/44f9512f-d972-4804-9a5e-a2db48f4f2aa)
