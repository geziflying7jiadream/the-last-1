# lingjing-game1
nanjingmajiang-game

# 本地开启redis-server.php
VM:
设置共享文件夹:www(本地共享文件夹)，
VM中网络：ipv4
          网络/添加ipv4：
          地址          子网掩码          网关
          192.168.2.8   255.255.255.0  192.168.2.254 
          DNS服务器
          192.168.1.11
挂在共享文件夹：sudo mount -t vboxsf www(本地文件夹)   VM虚拟机上的共享文件夹路径         
共享项目文件夹目录下：执行启动swoole服务
文件夹$ /home/zmliu/php/bin/php ExtGameService.php
启动（redis开启）之后，运行时一致打开，
不用时ctrl+c退出

1.枣庄麻将
sudo mount -t vboxsf www /mnt/test_share

本机的配置：
cd /mnt/test_share/cgc_zaozhuang_majiang_service 
/home/zliu/php/bin/php ExtGameService.php
