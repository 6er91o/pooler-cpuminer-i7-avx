Miner compiled for i7 with AVX, some changes were made in configure to work (-V replaced with -v for gcc to work)

$ ./configure CFLAGS="-O3 -march=corei7-avx -pipe -mfpmath=sse -mtune=corei7-avx -flto"

https://bitcointalk.org/index.php?topic=55038.0

# --------- #
# Usage     #
# --------- #

$ ./minerd --url=http://myminingpool.com:9332 --userpass=my.worker:password
$ ./minerd --url=stratum+tcp://myminingpool.com:3333 --userpass=my.worker:password

# --------- #
# Platform  #
# --------- #

uname -m = i686
uname -r = 3.2.0-57-generic-pae
uname -s = Linux
uname -v = #87-Ubuntu SMP Tue Nov 12 21:57:43 UTC 2013

http://gcc.gnu.org/gcc-4.6/changes.html
http://wiki.gentoo.org/wiki/Safe_CFLAGS#Core_i3.2Fi5.2Fi7_IvyBridge

# --------- #
# Recompile #
# --------- #

make clean
./configure CFLAGS="-O3 -march=corei7-avx -pipe -mfpmath=sse -mtune=corei7-avx -flto"
