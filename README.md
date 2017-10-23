# smartcashdeb
Debian Install Package for the SmartCash Wallet
# Part 1 -
**If you are doing a fresh install and not an upgrade please start here to include bootstrap!**
### Let's go to your home directory, create the .smartcash folder and enter it.
```sh
cd ~/
mkdir .smartcash
cd .smartcash
```
### Now let's get you caught up on the blockchain (via my bootstrap)
 If you don't have unzip already
```sh
  sudo apt-get install unzip
```
#
Now let's download the zipped bootstrap

```sh
wget 'http://proteanx.com/smartcashblocksoct19.zip'
```
(This may take a minute to download the 135mb zip)
#
Unzip the contents and remove the zip file
```sh
unzip smartcashblocksoct19.zip
rm smartcashblocksoct19.zip
```
You should now have 2 new folders in your .smartcash folder (blocks & chainstate). You're ready to move onto the install.

# Part 2 Installing the SmartCash Debian Install Package
**If you are just upgrading and/or adding menu support please start here and skip the bootstrap!**
### Let's download the appropriate package for your OS
#
For 32-bit
```sh
cd ~/Downloads/
wget 'https://github.com/proteanx/smartcashdeb/releases/download/0.8.7.10/smartcash32_0.8.7.10.deb'
sudo dpkg -i smartcash32_0.8.7.10.deb
```
#
For 64-bit
```sh
cd ~/Downloads/
wget 'https://github.com/proteanx/smartcashdeb/releases/download/0.8.7.10/smartcash64_0.8.7.10.deb'
sudo dpkg -i smartcash64_0.8.7.10.deb
```

Your installation is now complete! You can now find the SmartCash Wallet in the 'Internet' section of your Desktop Menu or start the qt client by using the 'smartcash-qt' command in your terminal!
