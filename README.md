# KIInode
## Tutorial - Install KII node on Ubuntu Server

**Update your Ubuntu server with the following command:**

*sudo apt-get update && sudo apt-get upgrade -y*

**Install the required dependencies with the following command:**

*sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev libboost-program-options-dev libminiupnpc-dev libzmq3-dev libprotobuf-dev protobuf-compiler unzip software-properties-common cmake -y*

**Install the repository ppa:bitcoin/bitcoin with the following command:**

*sudo add-apt-repository ppa:bitcoin/bitcoin*

**Confirm the installation of the repository by pressing on the enter key. `enter`**

**Install Berkeley DB with the following command:**

*sudo apt-get update && sudo apt-get install libdb4.8-dev libdb4.8++-dev -y*

**Download the Linux daemon with the following command:**

*wget "https://github.com/kiiglobal/KII-Linux-daemon/blob/main/kii-daemon-linux.tar.gz" -O kii-daemon-linux.tar.gz*

**Extract the tar file with the following command:**

*tar -xzvf kii-daemon-linux.tar.gz*

**Download the Linux tools with the following command:**

*wget "https://github.com/kiiglobal/KII-Linux-wallet/blob/main/kii-qt-linux.tar.gz" -O kii-qt-linux.tar.gz*

**Extract the tar file with the following command:**

*tar -xzvf kii-qt-linux.tar.gz*

**Type the following command to install the daemon and tools:**

*sudo mv kiid kii-cli kii-tx /usr/bin/*

**Create the data directory for KII with the following command:**

*mkdir $HOME/.kii*

**Open nano.**

*nano $HOME/.kii/kii.conf -t*

**Paste the following into nano.**

*rpcuser=rpc_kii*
*rpcpassword=dR2oBQ3K1zYMZQtJFZeAerhWxaJ5Lqeq9J2*
*rpcbind=0.0.0.0*
*rpcallowip=127.0.0.1*
*listen=1*
*server=1*
*txindex=1*
*daemon=1*

**Save the file with the keyboard shortcut `ctrl` + `x`.**

**Type the following command to start your node:**

*kiid*
