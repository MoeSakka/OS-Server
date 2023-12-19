# Web Server
Web server adalah sebuah software (perangkat lunak) yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan HTTP atau HTTPS dari klien atau kita kenal dengan web browser (Chrome, Firefox, dan sebagainya). Selanjutnya ia akan mengirimkan respon atas permintaan tersebut kepada client dalam bentuk halaman web.
# Resource dan Service yang di Install
1. Ubuntu Server 20.04.4 LTS
2. SSH
3. Apache2
4. Firewall
5. Webmin
# Instalasi

1. Installing Apache2.
   
 - sudo apt update

 - sudo apt install apache2
   

2. Adjusting the Firewall.

 - sudo ufw app list

 - sudo ufw allow 'Apache'

 - sudo ufw status
   

3. Installing Webmin.

 - sudo apt update

 - sudo nano /etc/apt/sources.list

 - deb http://download.webmin.com/download/repository sarge contrib

 - wget -q -O- http://www.webmin.com/jcameron-key.asc | sudo apt-key add

 - sudo apt update

 - sudo apt install webmin

 - sudo ufw allow 10000
