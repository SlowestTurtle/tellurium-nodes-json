# tellurium-nodes-json
JSON List of public daemons for Tellurium

The json file in this repo contains the a list of known public nodes in which users can connect to sync their wallets.
Some of these may contain fees.

This list can be consumed in your application so you'll always have an up-to-date list of public nodes. To consume the list, use the following URL: https://github.com/TelluriumCoin/tellurium-nodes-json/blob/master/tellurium-nodes.json

Adding a New Node
If you would like to add your public node to the list, please submit a Pull Request to do so. To avoid any possibility of displaying preference for one public node over another, please ensure that any additions are submitted in alphabetical order by the name property.


# Creating your own public node

If you would like to create your own public node, here are the steps.

*What you’ll need:

1. A computer with an IP address that doesn’t change. If you’re running it from home and use cable or DSL internet, you’re probably already set up with a static IP. (Free Amazon servers or Google Cloud servers are perfect for this) 

2. A Tellurium wallet to collect your earnings. You can use a paper wallet or any other Tellurium wallet.  Make sure you have the keys to the wallet.

*Let’s Get Started

1. Connect to your node and install Tellurium. 
Dowload a pre-compiled deamon for windows or linux on https://github.com/telluriumcoin/tellurium/releases/
Or you can follow the compile guide on https://github.com/telluriumcoin/tellurium/
Create a folder and extract the compressed files into that folder.

2. Decide on a fee, and launch the daemon
Let’s say I want to charge 500.0000 TLRM per transaction sent, I can launch my daemon like this for linux:

./Telluriumd --p2p-bind-ip 0.0.0.0 --rpc-bind-ip 0.0.0.0 --fee-amount 5000000 --fee-address TELMfh3HwLaNBUMPpXWudjbciGYLeVVtYXdkpcdAye1GEvYkg2MJCSmPC76NAwf8dP1brBJCL9KDeENN8UAT45Vj5hbPgSKxdJ

For windows:
Telluriumd.exe --p2p-bind-ip 0.0.0.0 --rpc-bind-ip 0.0.0.0 --fee-amount 5000000 --fee-address TELMfh3HwLaNBUMPpXWudjbciGYLeVVtYXdkpcdAye1GEvYkg2MJCSmPC76NAwf8dP1brBJCL9KDeENN8UAT45Vj5hbPgSKxdJ

3. !! IMPORTANT !!
Release 2.0.1.0 New Updates
This version release allow anti-flood tools and features, please type HELP in node for further information or contact our team.

./Telluriumd --p2p-bind-ip 0.0.0.0 --rpc-bind-ip 0.0.0.0 --p2p-tx-threshold-count 10 --fee-amount 5000000 --fee-address TELMfh3HwLaNBUMPpXWudjbciGYLeVVtYXdkpcdAye1GEvYkg2MJCSmPC76NAwf8dP1brBJCL9KDeENN8UAT45Vj5hbPgSKxdJ

Note that Tellurium uses 4 decimal places to determine its' atomic units.  The decimal is not used by the Daemon.  It only understands units.  So a fee of 500.0000 TLRM equates to 5000000 atomic units.

*What Do We Do Next?

Get your node listed on Github so that people know you exist!
If you are unfamiliar with github, please contact us at discord or by email.
Email: admin@tellurium.network
Discord: https://discord.gg/VaXYX6z

