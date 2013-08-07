# Bypassing iOS signature on Jailbreaked iOS

## require
- ldid command (Link Identifer)
- gcc

~~~
$ apt-get install ldid
$ git clone git@github.com:haya14busa/ios-build
$ sudo mv /usr/bin/gcc /usr/bin/realgcc
$ sudo mv /usr/bin/arch /usr/bin/realarch
$ cd ios-build
$ chmod +x gcc arch
$ cp gcc /usr/bin/
$ cp arch /usr/bin/
~~~
