# Bookmark

## codec
* [leandromoreira ffmpeg-libav-tutorial](https://github.com/leandromoreira/ffmpeg-libav-tutorial.git)

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

 
