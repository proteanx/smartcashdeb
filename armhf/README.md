# Proteus SmartCash Wallet Daemon armhf binary built on Raspbian via Raspberry Pi 3 

Installation instructions -

$ sudo apt-get install libssl-dev libdb++-dev libminiupnpc-dev

$ sudo apt-get install libboost-dev libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libcurl4-openssl-dev

$ cd ~/

$ wget 'https://github.com/proteanx/smartcashdeb/raw/master/armhf/smartcashd'

$ sudo mv smartcashd /usr/bin/smartcashd

$ sudo chmod a+x /usr/bin/smartcashd


Make sure you have your smartcash.conf 

$ mkdir .smartcash && cd .smartcash

$ sudo nano smartcash.conf

Fill in smartcash.conf info (RPC User & PW) (save on exit ctrl+x -> y -> enter)

$ sudo chmod 600 smartcash.conf

Now run smartcashd and begin downloading the blockchain

$ smartcashd -daemon

wait a few minutes

$ smartcashd getinfo




