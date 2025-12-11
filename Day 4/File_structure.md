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

       /boot  Contains  static  files  for  the boot loader.  This directory holds only the files which are needed during the boot process.  The map installer and
              configuration files should go to /sbin and /etc.  The operating system kernel (initrd for example) must be located in either / or /boot.

       /dev   Special or device files, which refer to physical devices.  See mknod(1).

       /etc   Contains configuration files which are local to the machine.  Some larger software packages, like X11, can have their own subdirectories below /etc.
              Site-wide configuration files may be placed here or in /usr/etc.  Nevertheless, programs should always look for these files in /etc and you may have
              links for these files to /usr/etc.
