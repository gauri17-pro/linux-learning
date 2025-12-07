## Commands to get to know about your server:

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

