## Ethical Hacker

##### In this course, we will learn some basics of Network penetration Testing

##### Pre-req
- Download and install oracle [virtualBox](https://www.virtualbox.org/wiki/Downloads) or [VMware workstation](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html). 
- Download [kali-linux](https://www.kali.org/get-kali/) and mount it on your preferred hyper-visor. 
- - If you are on Windows, you may download [WSL](https://www.kali.org/get-kali/#kali-wsl) for Kali from [miscrosoft store](https://www.microsoft.com/en-us/p/kali-linux/9pkr34tncv07?activetab=pivot:overviewtab). 

##### Enable and turn services
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