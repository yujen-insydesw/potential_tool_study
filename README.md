# potential_tool_study

## WOL (Wake On Lan) 網絡喚醒遠端開機功能-在外就能讓電腦開機
https://www.intone.cc/2018/07/wol-wake-on-lan-%E7%B6%B2%E7%B5%A1%E5%96%9A%E9%86%92%E9%81%A0%E7%AB%AF%E9%96%8B%E6%A9%9F%E5%8A%9F%E8%83%BD/#google_vignette

## vscode remote develop (via ssh)

https://xenby.com/b/221-教學-使用-visual-studio-code-透過-ssh-進行遠端程式開發

https://xenby.com/b/221-%E6%95%99%E5%AD%B8-%E4%BD%BF%E7%94%A8-visual-studio-code-%E9%80%8F%E9%81%8E-ssh-%E9%80%B2%E8%A1%8C%E9%81%A0%E7%AB%AF%E7%A8%8B%E5%BC%8F%E9%96%8B%E7%99%BC)

## vscode short cut

### rename symbol
...

### add selection match
crtl + D

### duplicate line
<img width="382" alt="duplicate_lines" src="https://github.com/user-attachments/assets/0d9551a6-e7fb-42ef-b6ba-ccd5da6683b7">

### go to definition
ctrl + click

### find command
ctrl + shift + p

### toggle silde bar
ctrl + B

### go to line
crtl + G : line number

### reference
https://youtu.be/_4rSbklsVkk?si=guKC7-wlsy0pr3nb

## draw uml
https://bramp.github.io/js-sequence-diagrams/

## harckMD
https://hackmd.io/c/tutorials-tw/%2F%40docs%2Finterface-view-tw

## readme & uml
https://github.com/Zingam/UML-in-Markdown/blob/master/README.md

## wsl

normal install \
https://www.howtogeek.com/744328/how-to-install-the-windows-subsystem-for-linux-on-windows-11/?form=MG0AV3
```console
# list available version
wsl -l -o

# install
wsl --install
wsl --install -d <version name>

# install desktop (not yet workable)
sudo apt install ubuntu-gnome-desktop
# run (not yet workable)
startx

# another way to install desktop (still have some bugs)
# https://ivonblog.com/posts/run-linux-desktop-on-wsl/
```

a command that starts WSL 2 VM, exits, and WSL 2 VM and instance are left running:
```console
wsl --exec dbus-launch true
```

other references \
https://blog.csdn.net/qq_63432403/article/details/130297605
```console
wsl --shutdown 

wsl --export Ubuntu-22.04 "E:\Wsl\Ubuntu.tar" 

wsl --unregister Ubuntu-22.04 

wsl --import Ubuntu-22.04 "E:\Wsl" "E:\Wsl\Ubuntu.tar" 

Ubuntu2204 config --default-user golemon 
```

## wireshark

https://ithelp.ithome.com.tw/articles/10300987

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


ssh 設定
https://hackmd.io/@W855Yo-6R22n28iWVYZdVw/HJwUo8yzT

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


## virtual box

### internet bride setting

how to set
https://www.youtube.com/watch?v=rhFLfwZzlGA

## Install common dev tool

### for ifconfig
sudo apt install net-tools

### ssh
sudo apt install openssh-server openssh-clients

#### linux kernel header
sudo apt-get install linux-headers-$(uname -r)

### lib
sudo apt-get install libboost-all-dev libsystemd-dev

### language / compiler
sudo apt install git meson libtool pkg-config gcc g++ cmake npm python3 python3-pip python3-yaml python3-mako python3-inflection

## windows 工作排程

![1](https://github.com/user-attachments/assets/a2fd9884-9efe-4332-b9cd-c4fa887dd2a3)
![2](https://github.com/user-attachments/assets/6da9f5ec-d82b-494a-92fb-647af8b264a9)
![3](https://github.com/user-attachments/assets/72ab59d2-8460-4073-9477-228a9cf2e289)
