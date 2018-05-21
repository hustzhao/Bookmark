# Bookmark

##leixiaohua 

* [博客地址] (https://blog.csdn.net/leixiaohua1020)

* [simplest_mediadata_test] (https://github.com/leixiaohua1020/simplest_mediadata_test/tree/master/simplest_mediadata_test)

正在学习...


## codec
* [leandromoreira ffmpeg-libav-tutorial](https://github.com/leandromoreira/ffmpeg-libav-tutorial.git)  
编译命令:  
gcc -o 0_hello_world 0_hello_world.c -I../ffmpeg/output/include -L../ffmpeg/output/lib -lavformat -lavcodec -lswscale -lswresample -lavutil -lz -lm -lpthread -ldl -llzma

## tutorial

* [bogotobogo](http://www.bogotobogo.com)
* [ffmpeg-tutorial mpenkov] (https://github.com/mpenkov/ffmpeg-tutorial)

## codec

* [digital_video_introduction](https://github.com/leandromoreira/digital_video_introduction) (PDF)

* [libdash](https://github.com/bitmovin/libdash)  

环境搭建，回到12.04吧，先安装12.04,下载地址(http://releases.ubuntu.com/12.04/ubuntu-12.04.5-desktop-i386.iso)
更改源地址为: mirrors.hust.edu.cn
### Ubuntu 12.04
1. sudo apt-get install git-core build-essential cmake libxml2-dev libcurl4-openssl-dev
2. git clone git://github.com/bitmovin/libdash.git (git clone git://github.com/hustzhao/libdash.git)
3. cd libdash/libdash
4. mkdir build
5. cd build
6. cmake ../
7. make
8. cd bin
9. The library and a simple test of the network part of the library should be available now. You can test the network part of the library with
10. ./libdash_networkpart_test

#### QTSamplePlayer
Prerequisite: libdash must be built as described in the previous section.

1. sudo apt-add-repository ppa:ubuntu-sdk-team/ppa
2. sudo apt-add-repository ppa:canonical-qt5-edgers/ubuntu1204-qt5 (这个和官方的不一致，官方的貌似不行)
3. sudo apt-get update
4. sudo apt-get install qtmultimedia5-dev qtbase5-dev libqt5widgets5 libqt5core5 libqt5gui5 libqt5multimedia5 libqt5multimediawidgets5 libqt5opengl5 libav-tools libavcodec-dev libavdevice-dev libavfilter-dev libavformat-dev libavutil-dev libpostproc-dev libswscale-dev
5. cd libdash/libdash/qtsampleplayer
6. mkdir build
7. cd build
8. wget http://www.cmake.org/files/v2.8/cmake-2.8.11.2-Linux-i386.sh
9. chmod a+x cmake-2.8.11.2-Linux-i386.sh
10. ./cmake-2.8.11.2-Linux-i386.sh
11. ./cmake-2.8.11.2-Linux-i386/bin/cmake ../
12. make
13. ./qtsampleplayer


## QT 
 * [QT downlaod url](https://download.qt.io/archive/qt/)

## HbbTV
 * [HbbTV FRM](http://www.francescpinyol.cat/hbbtv.html)
 
## DIAL
 * [netflix dial-reference](https://github.com/Netflix/dial-reference)
 
 /usr/bin/ld: 找不到 -lcares
 sudo apt install libc-ares-dev
 make[1]: Entering directory '/home/zhaotq/github/dial-reference/server'
 /usr/bin/ld: nf_callbacks.o: relocation R_X86_64_32 against `.bss' can not be used when making a shared object; recompile with -fPIC
 
 %.o: %.c $(HEADERS)
	$(CC) -Wall -g -std=gnu99 $(CFLAGS) -c $*.c -o $*.o -fPIC
nf_callbacks_lib: nf_callbacks.o
	$(CC) -Wall -Werror -g nf_callbacks.o -o libnfCallbacks.so --shared -fPIC

 
