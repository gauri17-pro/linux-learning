## YOUR TASKS TODAY
- Install a new application from the online repositories
- Become familiar with some of the standard directories
- Look at the format and content of some configuration files.

#### Installation of application

- To update the repositories is important before searching or installing the applications from online repositories
  ```
  sudo apt update
  ```

- To search the packages using apt search specifically for Debian distros like Ubuntu. For example:
  ```
  apt search "Midnight commander"
  ```
  <img width="1043" height="723" alt="image" src="https://github.com/user-attachments/assets/3865dd55-2c9d-4931-9d31-ce81db712905" />

- This will show a range of matching “packages”, and we can then install them with apt install command. So to install package mc (Midnight Commander) on Ubuntu:
  ```
  sudo apt install mc 
  ```

#### Linux directories

A typical Linux system has, among others, the following directories:

       /      This is the root directory.  This is where the whole tree starts.

       /bin   This directory contains executable programs which are needed in single user mode and to bring the system up or repair it.

       /boot  Contains  static  files  for  the boot loader.  This directory holds only the files that are needed during the boot process.  The map installer and
              configuration files should go to /sbin and /etc.  The operating system kernel (initrd for example) must be located in either / or /boot.

       /dev   Special or device files, which refer to physical devices. 

       /etc   Contains configuration files which are local to the machine.  Some larger software packages, like X11, can have their own subdirectories below /etc.
              Site-wide configuration files may be placed here or in /usr/etc.  Nevertheless, programs should always look for these files in /etc and you may have
              links for these files to /usr/etc.

       /home  On machines with home directories for users, these are usually beneath this directory, directly or not.  The structure of this directory depends  on
              local administration decisions (optional).
      
       /lib   This directory should hold those shared libraries that are necessary to boot the system and to run the commands in the root filesystem.

       /lost+found This directory contains items lost in the filesystem.  These items are usually chunks of files mangled as a consequence of a faulty disk or a           system crash.

       /media This  directory  contains mount points for removable media such as CD and DVD disks or USB sticks.  On systems where more than one device exists for
        mounting a certain type of media, mount directories can be created by appending a digit to the name of those available above starting with '0',  but the            unqualified name must also exist.

       /mnt   This  directory  is  a mount point for a temporarily mounted filesystem.  In some distributions, /mnt contains subdirectories intended to be used as
              mount points for several temporary filesystems.

       /opt   This directory should contain add-on packages that contain static files.

       /proc  This is a mount point for the proc filesystem, which provides information about running processes and the kernel.   This  pseudo-filesystem  is               described in more detail in proc(5).

       /root  This directory is usually the home directory for the root user (optional).

       /run   This  directory contains information which describes the system since it was booted.  Once this purpose was served by /var/run and programs may               continue to use it.

       /sbin  Like /bin, this directory holds system binaries 

       /srv   This directory contains site-specific data that is served by this system.

       /sys   This is a mount point for the sysfs filesystem, which provides information about the kernel like /proc, but better structured, following the formal‐
              ism of kobject infrastructure.

       /tmp   This directory contains temporary files which may be deleted with no notice, such as by a regular job or at system boot up.

       /usr   This directory is usually mounted from a separate partition.  It should hold only shareable, read-only data, so that it can be  mounted  by  various
              machines running Linux.

       /var   This directory contains files which may change in size, such as spool and log files.

        

        

       

      
      
