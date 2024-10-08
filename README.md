# potential_tool_study

## draw uml
https://bramp.github.io/js-sequence-diagrams/

## harckMD
https://hackmd.io/c/tutorials-tw/%2F%40docs%2Finterface-view-tw

## readme & uml
https://github.com/Zingam/UML-in-Markdown/blob/master/README.md

## wsl
https://blog.csdn.net/qq_63432403/article/details/130297605

wsl --shutdown 

wsl --export Ubuntu-22.04 "E:\Wsl\Ubuntu.tar" 

wsl --unregister Ubuntu-22.04 

wsl --import Ubuntu-22.04 "E:\Wsl" "E:\Wsl\Ubuntu.tar" 

Ubuntu2204 config --default-user golemon 

## vmware
1. **Enable Intel VT-x in BIOS**:
    - Restart your computer and enter the BIOS setup utility (usually by pressing a key like F2 or Del during startup).
    - Look for an option related to virtualization technology (often labeled as “Intel VT-x” or similar). Enable it.
    - Save the changes and exit the BIOS.
### vmware 16
https://vmware-workstation.informer.com/download/
https://github.com/pashayogi/VMware-Workstation-Pro-16-license-keys
![Untitled](https://github.com/user-attachments/assets/820e9b11-78db-4914-b2ad-069e0691f7ee)

### vmware tool (for drap and ... / copy and paste)
<img width="528" alt="螢幕擷取畫面 2024-08-23 144258" src="https://github.com/user-attachments/assets/7d6e2bb6-bb55-4ea9-be7d-36ed42f9cd81">

### openssh

安裝 OpenSSH 服務：
sudo apt-get update
sudo apt-get install openssh-server

啟動 SSH 服務
sudo systemctl start ssh

設置 SSH 服務開機自啟
sudo systemctl enable ssh

確認 SSH 服務已經正常運行：
sudo systemctl status ssh

### check firewall

nc -z -v <ip> <port:20-80>

Test-NetConnection -ComputerName 192.168.174.128 -Port 22

- Open a Specific Port
sudo ufw enable

- Allow a Specific Port (e.g., port 22 for SSH):
sudo ufw allow 22/tcp

- Allow a Range of Ports (e.g., ports 1000 to 2000):
sudo ufw allow 1000:2000/tcp

- Allow a Port for a Specific Service (e.g., HTTP):
sudo ufw allow http

- Open All Ports
sudo ufw disable

- Check Firewall Status
sudo ufw status
