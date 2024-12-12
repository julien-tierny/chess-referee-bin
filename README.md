# chess-referee-bin

This repository contains instructions for installing and running a binary distribution of a chess referee program, accompanied by a few sample chess playing programs.

# Downloads

## Ubuntu packages
 - [Ubuntu 20.04](packages/ubuntu/chesslib-ubuntu-20.04.deb.zip)
 - [Ubuntu 22.04](packages/ubuntu/chesslib-ubuntu-22.04.deb.zip)
 - [Ubuntu 24.04](packages/ubuntu/chesslib-ubuntu-24.04.deb.zip)

## MacOS packages
 - [Mac OS 13](packages/macos/chesslib-macos-13.tar.gz.zip)
 - [Mac OS 14](packages/macos/chesslib-macos-14.tar.gz.zip)
 - [Mac OS 15](packages/macos/chesslib-macos-15.tar.gz.zip)

## Windows
 - [Windows 2022](packages/windows/chesslib.exe.zip)

# Installation

## Ubuntu 
In the following, we assume you downloaded your package in the **current** directory (please move to the directory where you downloaded the package otherwise).
```
unzip chesslib*zip
sudo apt install ./chesslib.deb
```

## MacOS
In the following, we assume you downloaded your package in the **current** directory (please move to the directory where you downloaded the package otherwise).
```
unzip chesslib*zip
tar xvzf chesslib.tar.gz
sudo cp -R chesslib/* /usr/local
```

## Windows
In the following, we assume you downloaded your package in the **current** directory (please move to the directory where you downloaded the package otherwise).
```
unzip chesslib.exe.zip
chesslib.exe /S
```
