## GENERAL INFORMATION ABOUT THE SERVER

- To print the Linux Standard Base version and distributions.
```
lsb_release -a
```
<img width="1056" height="428" alt="ScreenShot 2025-12-07 at 20 51 45@2x" src="https://github.com/user-attachments/assets/e76bc2f8-aa49-4b10-9517-f25c36f6851b" />

-  lsb_release may not be available in your server, as it’s not widely adopted, but you will always have the same information available in the system file os-release. You can check its content by typing cat /etc/os-release
```
cat /etc/os-release
```
 <img width="2068" height="868" alt="ScreenShot 2025-12-07 at 20 54 23@2x" src="https://github.com/user-attachments/assets/c6d0d49a-f78a-4f01-a8a5-e8ddb43267dc" />

- To view the system information along with kernel version and hardware details use the command below:
```
uname -a
```
<img width="2934" height="204" alt="ScreenShot 2025-12-07 at 20 58 51@2x" src="https://github.com/user-attachments/assets/8f09f263-9bfc-4d09-97d6-e0cab9b3a271" />

- To get the details for how long your system is up and running
```
uptime
```
<img width="2228" height="220" alt="ScreenShot 2025-12-07 at 21 01 26@2x" src="https://github.com/user-attachments/assets/d7d77762-d991-40b0-a1e0-72de9a169471" />

- To know the current username
```
whoami
```
<img width="1780" height="230" alt="ScreenShot 2025-12-07 at 21 04 56@2x" src="https://github.com/user-attachments/assets/54140e87-1e37-46b4-b972-295eb42931d8" />

- To know who has logged in
```
who
```
<img width="1698" height="254" alt="ScreenShot 2025-12-07 at 21 15 18@2x" src="https://github.com/user-attachments/assets/8701bea0-3a1d-48b0-978c-77e396251969" />

- To know what the logged in users are doing
```
w
```
<img width="2124" height="374" alt="ScreenShot 2025-12-07 at 21 16 15@2x" src="https://github.com/user-attachments/assets/4a46596f-110b-4f85-8135-6d6663c7d053" />

## HARDWARE INFORMATION

- To know the hardware configuration details
```
lshw
```
<img width="1908" height="1088" alt="ScreenShot 2025-12-07 at 21 26 49@2x" src="https://github.com/user-attachments/assets/e6ff5110-3d6c-4c25-a910-f8f2eb857da4" />

- To view the CPU architecture
```
lscpu
```
<img width="2940" height="1304" alt="ScreenShot 2025-12-07 at 21 31 32@2x" src="https://github.com/user-attachments/assets/a9f38606-5642-4eb6-9e2a-8932b4f6b168" />

- To list the block devices
```
lsblk
```
<img width="1610" height="704" alt="ScreenShot 2025-12-07 at 21 33 14@2x" src="https://github.com/user-attachments/assets/1c26fe68-623e-4bc9-9977-d3bb18fc17f8" />

- To list the PCI devices
```
lspci
```
<img width="2008" height="534" alt="ScreenShot 2025-12-07 at 21 35 32@2x" src="https://github.com/user-attachments/assets/4cca73be-7004-4502-b4b6-8b962a7222cc" />

- To list the USB devices
```
lsusb
```

## MEMORY AND CPU USAGE 

- To check the amount of memory being used
```
free -h 
```
<img width="2192" height="344" alt="ScreenShot 2025-12-07 at 21 45 06@2x" src="https://github.com/user-attachments/assets/ed21e344-0c67-4ea7-8475-5052fbcf0511" />

- To check the VM statistics
```
vmstat
```
<img width="2206" height="350" alt="ScreenShot 2025-12-07 at 21 46 27@2x" src="https://github.com/user-attachments/assets/18a5687f-3b5f-4879-91bf-60d9ef0b0dba" />

- To check the CPU usage
```
top
```
<img width="2562" height="1582" alt="ScreenShot 2025-12-07 at 21 47 25@2x" src="https://github.com/user-attachments/assets/35811149-81c0-45f1-bc83-bc58dd6c25db" />

- To check the CPU usage in an interactive mode
```
htop
```
<img width="2562" height="1582" alt="ScreenShot 2025-12-07 at 21 47 25@2x" src="https://github.com/user-attachments/assets/ff894eef-9449-47d0-8abd-bc55874b5752" />

## MEASURE DISK SPACE USAGE

- To measure the disk space usage
```
df -h
```
<img width="1620" height="624" alt="ScreenShot 2025-12-07 at 21 50 32@2x" src="https://github.com/user-attachments/assets/e7258581-9288-439b-8a2a-a8f59d64c2d2" />

## MEASURE NETWORK USAGE 

- To check the IP address and get the general idea of your network interfaces
( Need to install net-tools package)
```
ifconfig
```
<img width="2092" height="1170" alt="ScreenShot 2025-12-07 at 22 00 21@2x" src="https://github.com/user-attachments/assets/62d463e7-05da-4ff0-8e9e-fafeb8f9c761" />

- netstat -i is used to display the network interfaces on your Linux system along with their statistics.
```
netstat -i
```
<img width="2316" height="468" alt="ScreenShot 2025-12-07 at 22 01 50@2x" src="https://github.com/user-attachments/assets/1d6fa9e6-fa7b-4824-a886-6d53aee0f437" />

- The command below shows all listening ports along with the program name and PID.
```
netstat -tulnp
```
<img width="2456" height="850" alt="ScreenShot 2025-12-07 at 22 06 08@2x" src="https://github.com/user-attachments/assets/93477509-6f3d-4f13-96c3-59b365965909" />

