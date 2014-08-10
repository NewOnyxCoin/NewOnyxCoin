*Onyxcoin V2 - X13 CryptoCurrency
*RPC Port: 51990
*P2P Port: 50990
*Algorithm: X13 POW/POS starts on block 15,000
*Ticker: ONYX
*Max PoW Coins: Approx. ~15,000,000
*5% PoS Annual Interest

*X13 Hashing Algorithm:(blake, bmw, groestl, jh, keccak, skein, luffa, cubehash, shavite, simd, echo, hamsi, fugue)

*Block Reward Schedule:
*No Pre-Mine
*Block 0-50 are low reward test blocks to prevent insta-mine
*Block 50-15,000 are 1,000
*PoW Ends on Block 15,000 (approx. 10 days)

*PoS Starts on Block 2, MinStakeAge: 24 hours, MaxStakeAge: Unlimited, 5% Annual Interest

##Troubleshooting

In the event you encounter problems compiling the daemon, feel free to consult the guide below:

Receive the following error?

------------------------------------------

PROBLEM:

g++: error: /home/user/Desktop/onyx/OnyxCoin/src/leveldb/libleveldb.a: No such file or directory
g++: error: /home/user/Desktop/onyx/OnyxCoin/src/leveldb/libmemenv.a: No such file or directory

SOLUTION:

cd src/leveldb
make libleveldb.a libmemenv.a

CD back to src and try to build it again.

If you get the following error trying to do the above,

/bin/sh: 1: ./build_detect_platform: Permission denied
Makefile:18: build_config.mk: No such file or directory

chmod 755 src/leveldb/build_detect_platform

try again

------------------------------------------


