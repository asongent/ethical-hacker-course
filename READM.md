## Ethical Hacker

##### In this course, we will learn some basics of Network penetration Testing

1. ##### Pre-req
- Download and install oracle [virtualBox](https://www.virtualbox.org/wiki/Downloads) or [VMware workstation](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html). 
- Download [kali-linux](https://www.kali.org/get-kali/) and mount it on your preferred hyper-visor. 
- - If you are on Windows, you may download [WSL](https://www.kali.org/get-kali/#kali-wsl) for Kali from [miscrosoft store](https://www.microsoft.com/en-us/p/kali-linux/9pkr34tncv07?activetab=pivot:overviewtab). 

2. ##### Install git
- Run 
```bash
sudo apt install git -y 
```
3. ##### Remove and reinstall impacket
- Remove impacket by running the following
```bash 
sudo apt purge *impacket* -y
```
- clone and impacket from [impacket repo on git](https://github.com/SecureAuthCorp/impacket) and reinstall impacket
- - First `cd /opt/` directory and run 
```bash
git clone https://github.com/SecureAuthCorp/impacket.git
```

- - If you do no have python3 installed, run 
```bash
sudo apt install python3 -y
```
```bash
sudo install pip
```
- - Move to impacket folder(`cd impacket`) and reinstall ipacket
```bash
sudo python3 -m pip install .
```

4. ##### Enable and turn services
- Once the installation is completed, enable and turn on the following services.

```bash
sudo systemctl enable apache2
```
```bash
sudo service apache2 start
```
```bash
sudo systemctl enable ssh
```
```bash
sudo service ssh start
```
```bash
sudo systemctl enable postgresql
```
```bash
sudo service postgresql start
```