# Kali Linux XRDP Docker Image

### Overview

This Docker image is based on Kali Linux rolling release, configured to run an XRDP server with the XFCE desktop environment. It allows users to access a full Kali Linux GUI over RDP.

### Quick Start


##### Pull image
```
docker pull ghcr.io/warshipfucker/kali-xrdp:latest
```
##### Rename Docker image 
docker tag ghcr.io/warshipfucker/kali-xrdp:latest kali-xrdp:latest
##### Run container
Run command

```
docker run -it --name kali-linux -v C:\dev-env\volumes\kali/run:/run -v C:\dev-env\volumes\kali/home:/home -v C:\dev-env\volumes\kali/mnt:/mnt  -v C:\dev-env\volumes\kali/opt:/opt -p 3390:3389 -p 2222:22  -p 8081:8080 kali-xrdp:latest kali kali yes 
```
##### Develop 
Clone Repository: in progress.....
##### Connect
On your Windows Host
1. Press Win+R buttons
2. In "Run" window type **mstsc** and press Enter
3. In Remote Desktop Connection window type **localhost:3390**
4. Login via creditionals **kali:kali**

### Features

- XFCE Desktop Environment

- XRDP for remote desktop access

- Pre-installed tools for a productive environment

### License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/warshipfucker/kali-xrdp/LICENSE) file for details.
