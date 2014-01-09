Miner compiled for i7 with AVX, 32 bit

$ ./configure CFLAGS="-Ofast -march=corei7-avx -pipe -mfpmath=sse -funroll-loops -mtune=corei7-avx -flto" CXXFLAGS="${CFLAGS}"

https://bitcointalk.org/index.php?topic=55038.0

$ ./minerd -o stratum+tcp://abc.host.com:3333 -u myname -p mypass

http://gcc.gnu.org/gcc-4.6/changes.html
http://wiki.gentoo.org/wiki/Safe_CFLAGS#Core_i3.2Fi5.2Fi7_IvyBridge
