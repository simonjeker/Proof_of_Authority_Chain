# Proof_of_Authority_Chain

##Step by step instructions

Setup the custom out-of-the-box blockchain


Create a new project directory for your new network. Call it whatever you want!


Create a "Screenshots" folder inside of the project directory.


Create accounts for two (or more) nodes for the network with a separate datadir for each using geth.


Run puppeth, name your network, and select the option to configure a new genesis block.


Choose the Clique (Proof of Authority) consensus algorithm.


Paste both account addresses from the first step one at a time into the list of accounts to seal.


Paste them again in the list of accounts to pre-fund. There are no block rewards in PoA, so you'll need to pre-fund.


You can choose no for pre-funding the pre-compiled accounts (0x1 .. 0xff) with wei. This keeps the genesis cleaner.


Complete the rest of the prompts, and when you are back at the main menu, choose the "Manage existing genesis" option.


Export genesis configurations. This will fail to create two of the files, but you only need networkname.json.


You can delete the networkname-harmony.json file.





Initialize each node with the new networkname.json with geth.

