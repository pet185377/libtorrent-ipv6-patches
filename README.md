libtorrent-ipv6-patches
=======================

IPv6 patches for recent versions of rakshasa libTorrent.

Do not use HEAD if you plan to use ruTorrent.


Pre-patched archive (using the latest tar from http://libtorrent.rakshasa.no/downloads/): https://flowerserv.net/upload/libtorrent.tar.gz

这个补丁包存在一行代码的错误

1. 下载到解压出的libtorrent文件夹中

2. nano 你的相应路径/src/net/socket_fd.cc

2. patch -p1<lib_ipv6.patch

3. 然后跳转到第123行，删除 printf(“Unable to open ipv6 socket\n”); 

