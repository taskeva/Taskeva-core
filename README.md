Taskeva Coin (TASK) integration/staging repository
======================================

TaskevaCoin is a cutting edge cryptocurrency, with many features not available in most other cryptocurrencies.
- Anonymized transactions using zerocoin technology.
- Fast transactions featuring guaranteed zero confirmation transactions named _SwiftX_.
- Decentralized blockchain voting providing for consensus based advancement of the current Masternode
  technology used to secure the network and provide the above features, each Masternode is secured
  with a collateral of 1.000.000 TASK.


Quick installation of the Taskeva daemon under linux.

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/taskeva/Taskeva-core.git
    cd Taskeva-core
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip taskevad
    sudo strip taskeva-cli
    sudo strip taskeva-tx
    cd ..

Running the daemon:

    taskevad

Stopping the daemon:

    taskevad stop

Demon status:

    taskevad getinfo
    taskevad mnsync status



More information at [Taskeva.com](https://go.taskeva.com)


### Coin Specs
<table>
<tr><td>Algo</td><td>Quark</td></tr>
<tr><td>Block Time</td><td>60 Seconds</td></tr>
<tr><td>Block Split</td><td>60% MN / 40% Staking</td></tr>
<tr><td>Difficulty Retargeting</td><td>Every Block</td></tr>
<tr><td>Max Coin Supply</td><td>4.000.000.000 TASK</td></tr>
<tr><td>Masternode collateral</td><td>1.000.000 TASK</td></tr>
<tr><td>P2P port</td><td>22203</td></tr>
<tr><td>RPC port</td><td>22202</td></tr>
</table>