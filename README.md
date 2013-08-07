# Bypassing iOS code signature on Jailbreaked on iOS5 and maybe iOS6

- First, you need to add cydia repository
    - http://cydia.radare.org
    - from this repo install libgcc
    - (this repo is **not** for cracked app but for developer)
- And install terminal.app or OpenSSH and Apt7

on iOS
~~~
$ sudo apt-get install ldid libgcc
$ sudo apt-get install make python coreutils inetutils git 
$ git clone git@github.com:haya14busa/ios-build
$ sudo mv /usr/bin/gcc /usr/bin/realgcc
$ sudo mv /usr/bin/arch /usr/bin/realarch
$ cd ios-build
$ chmod +x gcc arch
$ sudo cp gcc /usr/bin/
$ sudo cp arch /usr/bin/
$ sudo ldid -S /usr/bin/gcc
$ sudo ldid -S /usr/bin/arch
~~~

Now you can use ./configure or make so compile anything you want!

## Link
- [Need to disable codesign](http://ininjas.com/forum/index.php?topic=1626.msg46557)
- [Setup gcc On iPhone 4S running iOS 5 - RC.Z](https://rc-z.me/blog/archives/2012/02/29/setup-gcc-on-iphone-4s-running-ios-5/)
- [How To: Set up GCC on iOS 4 — n8.io](http://n8.io/how-to-set-up-gcc-on-ios-4/)
