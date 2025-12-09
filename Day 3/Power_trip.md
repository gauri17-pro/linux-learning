- Root user is the user with maximum permissions.

- It is the most powerful user in any Linux system with all the privileges to operate.

- In ancient times, sysadmins used to login as root in production systems, but it’s now common Best Practice to discourage or disallow login directly by root and instead to give specified trusted users the permission to run root-only commands via the sudo command.

- sudo -i: To launch a default user with super privileges which also loads root's environment 

- sudo {command}: Executes the command as a root user

- sudo -s: Opens a shell as root but keeps your current environment

#### TASKS FOR TODAY

- Change the password of sudo user
```
sudo passwd {username}
```

- Also learnt about TLDR
  tldr stands for “Too Long; Didn’t Read.”
  It is a command-line tool that gives short, simplified, practical examples of Linux commands — unlike long and complex man pages.

  For installing tldr:
  1. sudo apt update
  2. sudo apt install tldr
  3. Create a directory at location ~/.local/share/tldr
  4. tldr --update

- Change the hostname
  hostnamectl will provide the current hostname of the system along with other system details
  ```
  hostnamectl
  ```
  <img width="581" height="408" alt="image" src="https://github.com/user-attachments/assets/6b07e357-11d1-4325-b213-56ba63be6407" />


  In order th change the hostname we use the command:
  ```
  sudo hostnamectl set-hostname 'LoTR-universe'
  ```
  <img width="882" height="441" alt="image" src="https://github.com/user-attachments/assets/533357ab-c25b-4d63-91a1-235cd9977f08" />

- Change the timezone
  Command below gives the timezone of the system 
  ```
  timedatectl
  ```
  <img width="711" height="282" alt="image" src="https://github.com/user-attachments/assets/1b5ac956-fa47-4718-b31d-b37f2ad53915" />

  To list all possible timezones we use the command below
  ```
  timedatectl list-timezones
  ```
  <img width="683" height="470" alt="image" src="https://github.com/user-attachments/assets/1976736f-502d-47cc-b778-28a2a9102e76" />

  To set the timezone to IST
  ```
  sudo timedatectl set-timezone Asia/Kolkata
  ```
  <img width="876" height="280" alt="image" src="https://github.com/user-attachments/assets/0f3e610e-4824-4756-b46a-e2892f7288f5" />

## LOCAL CHANGES VS GLOBAL CHANGES

- Global changes: Programs/Environments that can be used across the system by any user. A global change affects all users.

- Local changes: Programs/Environments specific to particular user within the system which is not available for other users. A local change affects only one user.

## TYPES OF USERS IN LINUX

-  root user: The superuser (UID 0) with unrestricted power.

-  system users (Service Accounts)
   Users with the UID range 1-999 that are created for services like mysql, daemon
   These are not real human users.
   Used to isolate and secure background processes.

-  non-root or regular users:
   Normal accounts with restricted access to their own files.
   They cannot make system-wide changes unless given special privileges.

The following image shows all the users on the system:
<img width="837" height="746" alt="image" src="https://github.com/user-attachments/assets/ec5ccdf6-77f8-4ba4-99d0-8e2abd0a6367" />

## Note: Not a good practice to log in as root

## SUDOERS 

- Regular users who are granted extra privileges through the sudoers file are known as sudo-enabled users or sudoers.
- They can run some or all administrative commands as root (depending on their configuration).
- It’s common to have at least one sudoer that has the same powers as root, but the amount of privileges other sudoers have can vary.

- Method 1: You can provide sudo access to the regular user by adding that user to the sudo or wheel group using the command:
  ```
  usermod -a -G sudo ${username}
  ```

- Method 2: This can also be achieved by adding that regular user to the /etc/sudoers file.
  ```
  username ALL=(ALL) ALL
  ```

- Method 3: Create a Custom Rule in /etc/sudoers.d/
  ```
  sudo vi /etc/sudoers.d/username
  ```
  Add the rule:
  ```
  username ALL=(ALL) ALL
  ```
  The file must have the correct permissions
  ```
  sudo chmod 440 /etc/sudoers.d/username
  ```

## THE POWER OF SUDO


  


