bitcoinex v0.9.0.2
================================

http://www.btceproject.com

Copyright (c) 2009-2014 Bitcoin Developers

Copyright (c) 2017 bitcoinex Foundation

What is bitcoinex?
----------------

bitcoinex is an experimental crypto currency that uses scrypt as a proof-of-work algorithm.

 - 1 minute block targets
 - subsidy reduces in stages depending on current coin supply (50,25,10,5,1,0)
 - 100,000,000 total coins
 - Retargets every block using Dark Gravity Wave 3


Build Instructions
------------------

```
cd bitcoinex
qmake
make
```

See [docs](https://github.com/btceproject/bitcoinex/tree/master/doc) for flags, deps and more info.


Compiled Binaries Instructions
------------------------------

Precompiled Windows and Nix binaries available at https://btceproject.com

See instructions below.


Windows Setup
--------------------

- Double click the setup.exe file to install automatically

- Alternatively run **bitcoinex-qt.exe** or **bitcoinexd.exe** without using the installer

If the wallet doesn't automatically start syncing you will need to create a 
.conf file.

1) Close the Wallet / Daemon

2) Create a new text file

3) Inside paste the following (*changing the user and password*) :

```
rpcuser=ChooseAUserName
rpcpassword=ChooseAStrongRandomPassword
addnode=35.189.126.61
addnode=144.217.242.223

```

4) Save the file as **bitcoinex.conf**

5) Place it inside the following DIR :

```
/Users/<username>/AppData/Roaming/bitcoinex
```

6) Restart Wallet / Daemon


Nix Setup
--------------------

1) Navigate to the folder where bitcoinexd is and run it :

```
./bitcoinexd -daemon
```

bitcoinex server will start and then stop saying it needs a missing config file.

In the folder you downloaded will find a file called **bitcoinex.conf.example.txt**

Open it and put your user and password in the correct places then save the file as **bitcoinex.conf**

Put this file in the following folder : 

```
.bitcoinex
```
          
It's a hidden folder click ctrl + H to display hidden folders if you can't see it.


bitcoinex-qt (The GUI Wallet)
------------------------

This is NOT a static build. It requires external libraries for it to work. If you have built other wallets on your computer before, the chances are that you will already have all of the required libraries. If not see the build [docs](https://github.com/btceproject/bitcoinex/tree/master/doc).


For more information, as well as pre-compiled versions of the latest bitcoinex client sofware visit http://www.btceproject.com

Official bitcoinex Mining pool : http://pool.btceproject.com

bitcoinex Block Explorer : http://explorer.btceproject.com


License
-------------------

Developers work in their own trees, then submit pull requests when they think their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the bitcoinex development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't match the project's coding conventions (see `doc/coding.txt`) or are controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be completely stable. [Tags](https://github.com/btceproject/bitcoinex/tags) are created regularly to indicate new official, stable release versions of bitcoinex.


Disclaimer
-------------------

bitcoinex is an entirely experimental project and we offer no warranties or guarantees.
Use entirely at your own risk.

