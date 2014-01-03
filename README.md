Miner compiled for i7 with AVX

$ ./configure CFLAGS="-O3 -march=corei7-avx -pipe -mfpmath=sse -mtune=corei7-avx -flto"

https://bitcointalk.org/index.php?topic=55038.0

$ ./minerd --url=http://myminingpool.com:9332 --userpass=my.worker:password
$ ./minerd --url=stratum+tcp://myminingpool.com:3333 --userpass=my.worker:password

http://gcc.gnu.org/gcc-4.6/changes.html
http://wiki.gentoo.org/wiki/Safe_CFLAGS#Core_i3.2Fi5.2Fi7_IvyBridge

make clean
./configure CFLAGS="-O3 -march=corei7-avx -pipe -mfpmath=sse -mtune=corei7-avx -flto"
