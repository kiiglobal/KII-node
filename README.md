# KIInode
## Tutorial - Install KII node on Ubuntu Server

**Update your Ubuntu server with the following command:

*sudo apt-get update && sudo apt-get upgrade -y

**Install the required dependencies with the following command:

*sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev libboost-program-options-dev libminiupnpc-dev libzmq3-dev libprotobuf-dev protobuf-compiler unzip software-properties-common cmake -y

**Install the repository ppa:bitcoin/bitcoin with the following command:

*sudo add-apt-repository ppa:bitcoin/bitcoin

**Confirm the installation of the repository by pressing on the enter key. *enter

**Install Berkeley DB with the following command:

*sudo apt-get update && sudo apt-get install libdb4.8-dev libdb4.8++-dev -y
