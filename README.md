Установочный скрипт 3proxy для VPS на Debian / Ubuntu
======================================================

Простой скрипт 3proxy на Ubuntu/Debian

**MANUAL :**

Установка :

    wget --no-check-certificate https://raw.githubusercontent.com/DarkFort/3proxy/master/3proxyinstall.sh
    chmod +x 3proxyinstall.sh
    ./3proxyinstall.sh

Настройте авторизацию!!! 

    nano /etc/3proxy/.proxyauth
	
Например .proxyauth

    johndoe:CL:johndoepassword123

Настройте порт HTTP/SOCKS, по умолчанию порт 9999 (HTTP) и 8088 (SOCKS)

    nano /etc/3proxy/3proxy.cfg
    

Start service (or reboot as it's automatically start)

    service 3proxy start
	
Uninstall:

	wget --no-check-certificate https://raw.github.com/SnoyIatk/3proxy/master/3proxyuninstall.sh
	chmod +x 3proxyuninstall.sh
	./3proxyuninstall.sh

**Script tested on 04.06.2017 on EC2 AMI :**

- Ubuntu 16.04 64bit

**Script will run on :**
- Debian 6 32bits
- Debian 7 32bits
- Ubuntu 12.10 32bits
- Ubuntu 12.04 32bits
- Ubuntu 14.04 and later
