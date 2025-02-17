# chess-referee-bin

This repository contains instructions for installing and running a binary distribution of a chess referee program, accompanied by a few sample chess playing programs.

# Downloads

## Ubuntu packages
 - [Ubuntu 20.04](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/ubuntu/chesslib-ubuntu-20.04.deb.zip)
 - [Ubuntu 22.04](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/ubuntu/chesslib-ubuntu-22.04.deb.zip)
 - [Ubuntu 24.04](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/ubuntu/chesslib-ubuntu-24.04.deb.zip)

## MacOS packages
 - [Mac OS 13](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/macos/chesslib-macos-13.tar.gz.zip)
 - [Mac OS 14](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/macos/chesslib-macos-14.tar.gz.zip)
 - [Mac OS 15](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/macos/chesslib-macos-15.tar.gz.zip)

## Windows
 - [Windows 2022](https://github.com/julien-tierny/chess-referee-bin/raw/refs/heads/main/packages/windows/chesslib.exe.zip)

# Installation

In the following, we assume you downloaded your package in the **current** directory (please move to the directory where you downloaded the package otherwise).

## Ubuntu 
```
unzip chesslib*zip
sudo apt install ./chesslib.deb
```

## MacOS
```
unzip chesslib*zip
tar xvzf chesslib.tar.gz
sudo cp -R chesslib/* /usr/local
```

## Windows
```
unzip chesslib.exe.zip
chesslib.exe /S
```

# Playing a game against a random player
To make your program play a game against a random player, enter the following commands.
## Ubuntu
```
chessGame -W <path to your program> -B chessRandomPlayer
```

## MacOS
```
chessGame -W <path to your program> -B chessRandomPlayer
```

## Windows
```
set PATH=%PATH%;C:\Program Files\chesslib\bin\
chessGame.exe -W <path to your program> -B chessRandomPlayer.exe
```

# Collecting statistics against a random player
To play multiple games against a random player and retrieve statistics about
these games (e.g., percentage of legal games, percentage of wins, etc.), enter
the following commands.

## Ubuntu
```
chessStats -n <number of games> -p <path to your program> -o chessRandomPlayer
```

## MacOS
```
chessStats -n <number of games> -p <path to your program> -o chessRandomPlayer
```

## Windows
```
set PATH=%PATH%;C:\Program Files\chesslib\bin
chessStats.exe -n <number of games> -p <path to your program> -o chessRandomPlayer.exe
```
