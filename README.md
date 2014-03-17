


omegacoin.net



Technical Specifications
========================

 - Srypt proof-of-work algorithm
 - 60 second block time targets
 - ~100 billion total coins
 - 20,000 coins per block, halves every ~2 years
 - Retarget every 10 times per day (every 144 blocks)
 
UBUNTU DEPENDENCIES
===================
sudo apt-get install build-essential libboost-all-dev libcurl4-openssl-dev libdb5.1-dev libdb5.1++-dev git qt-sdk libminiupnpc-dev

sudo apt-get install qrencode libqrencode-dev 

UBUNTU COMPILE omegacoind
========================
cd ~

git clone git://github.com/omegacoinproject/omegacoin.git

cd /omegacoin/src

make -f makefile.unix USE_UPNP=-

sudo cp omegacoind /usr/bin


When trying to compile if you get this error: "../share/genbuild.sh: 34: ../share/genbuild.sh: cannot create obj/build.h: Directory nonexistent
make: *** [obj/build.h] Error "

Make sure to create the folder "obj" in the "src" folder:

cd /omegacoin/src

mkdir obj

Then try compiling again.


UBUNTU COMPILE omegacoin-qt
========================
cd omegacoin

qmake "USE_UPNP=-" omegacoin-qt.pro

make

Links
======

Website: http://www.omegacoin.net

OmegacoinTalk: http://omegacointalk.com/index.php

BitcoinTalk: https://bitcointalk.org/

Facebook: https://www.facebook.com/omegacoincoin

Twitter: https://twitter.com/omegacoincoinOMG

VK: https://vk.com/omegacoin

Reddit: http://www.reddit.com/r/omegacoin/

IRC Channel: http://webchat.freenode.net/?channels=#omegacoincoin



