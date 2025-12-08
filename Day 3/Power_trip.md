- Root user is the user with maximum permissions.

- It is the most powerful user n any Linux system with all the privileges to operate.

- In ancient times, sysadmins used to login as root in production systems, but it’s now common Best Practice to discourage or disallow login directly by root and instead to give specified trusted users the permission to run root-only commands via the sudo command.

- sudo : To execute a command as another user

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

