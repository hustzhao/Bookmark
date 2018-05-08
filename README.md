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

 
