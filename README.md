-----------------------------   
##  ServerSpeeder Install     
-----------------------------      
----------------------------- 
# For Linux (simple)   
Usage    
```
Usage:     
      bash appex.sh [install |uninstall |install '{serverSpeeder of Kernel Version}']     
```
Install
```
wget --no-check-certificate -O appex.sh https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh && chmod +x appex.sh && bash appex.sh install

```    
Uninstall    
```
wget --no-check-certificate -O appex.sh https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh && chmod +x appex.sh && bash appex.sh uninstall

```  
-----------------------------    
debian 降低内核安装锐速。
```    
wget http://snapshot.debian.org/archive/debian/20140310T221406Z/pool/main/l/linux/linux-image-3.12-1-amd64_3.12.9-1_amd64.deb  
wget http://snapshot.debian.org/archive/debian/20140310T221406Z/pool/main/l/linux/linux-headers-3.12-1-common_3.12.9-1_amd64.deb

```
安装内核
```    
dpkg -i *.deb

```
删除旧内核
```    
dpkg -l|grep linux-image | awk '{print $2}' #列出所有内核  
apt-get purge XXXXXXXXX -y #删除内核
```  
更新&重启
```    
update-grub   
reboot  
``` 

