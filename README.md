# Proxmox remove no-subscription message from ui

If you have no subscription and visit the webinterface it will popup a no-subscription message in the webui and you get warnings in the repository overview.  
This Script will disable this popup and remove the warnings in the repository overview.

It works for: 
* Proxmox Virtual Environment short PVE  
  PVE 6, 7 and 8
* Proxmox Backup Server short PBS
* Proxmox Mail Gateway Not Tested

Before:
![image](https://github.com/thethink3r/Proxmox-remove-no-subscription-message/assets/132231658/fa89042f-11a1-48d8-89da-37d86237db5f)

After:

![image](https://github.com/thethink3r/Proxmox-remove-no-subscription-message/assets/132231658/a8235b40-4b65-4731-b2fa-3aeb2cd91563)

Install:
```bash
# get apt script
wget -O /etc/apt/apt.conf.d/pve-no-subscription-message https://raw.githubusercontent.com/thethink3r/Proxmox-remove-no-subscription-message/main/pve-no-subscription-message

# for Browser
apt install --reinstall proxmox-widget-toolkit

# for Mobile 
apt install --reinstall pve-manager
```
