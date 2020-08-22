#如何设置无线网络
设置树莓派的无线网络（Wi-Fi）的方法有多种:  

##方法一，烧好SD卡后立刻设置
1.烧好SD卡后，把SD卡重新插入PC。  
  这时可以看到一个名为"boot"的U盘驱动器
1.在boot的根目录下面创建一个名为"ssh"的空文件，没有文件后缀。
1.再在boot的根目录下创建一个名为"wpa_supplicant.conf"的文件，内容如下
  ‘
country=CN
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
network={
    ssid="SSID"
    psk="WIFI密码"
}
  ’  
  注意：树莓派ZERO只能连2.4G的Wi-Fi，树莓派4可以连5G和2.4G两种
1.弹出SD卡  
1.把SD卡插入树莓派并启动，即可连上Wi-Fi


##方法二，待续...

