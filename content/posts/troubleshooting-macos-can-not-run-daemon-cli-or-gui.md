---
title: 'Troubleshooting MACOS can not run daemon CLI or GUI'
date: Thu, 08 Nov 2018 08:51:06 +0000
draft: false
tags: ['Articles', 'CLI', 'daemon', 'GUI Wallet', 'How to', 'MACOS', 'News and Announcement', 'Security', 'Technology', 'Troubleshooting', 'xeonbit', 'Xeonbit Updates']
toc: true
related: true
social_share: true
---

_“dyld: library not loaded: /usr/local/opt/zeromq/lib/libzmq.5.dylib”_ As you may see there is missing some library in the MAC OS system, we should install them by yourself to process the xeonbitd daemon: If you dont want to install Xcode then just skip it. Based on the error above you only need to install zeromq lib then we just install homebrew and zeromq. Depend on which package missing then we will apply for it.

1.  Install Xcode from AppStore
    
2.  Install [homebrew](http://brew.sh/)
    
3.  Install  xeonbit dependencies:
    

`brew install boost --c++11`

`brew install openssl` – to install openssl headers

`brew install pkgconfig`

`brew install cmake`

`brew install zeromq`

_Note_: If cmake can not find zmq.hpp file on OS X, installing `zmq.hpp` from [https://github.com/zeromq/cppzmq](https://github.com/zeromq/cppzmq) to `/usr/local/include` should fix that error.

`brew install qt5` (or download QT 5.8+ from [qt.io](https://www.qt.io/download-open-source/))

If you have an older version of Qt installed via homebrew, you can force it to use 5.x like so:

`brew link --force --overwrite qt5`

4.  Add the Qt bin directory to your path
    
    Example: `export PATH=$PATH:$HOME/Qt/5.11.1/clang_64/bin`
    
    This is the directory where Qt 5.x is installed on **your** system
    
    
    _“xcode-select: error: invalid developer directory ‘Library/Developer/CommandLineTools’ Failled durring: /usr/bin/sudo /usr/bin/xcode-select –switch /Library/Developer/ComandLineTools”_
    
     Run the following commands to fix the above errorsudo xcode-select –install sudo xcode-select -switch / I found the answer on [https://github.com/Homebrew/homebrew/issues/23500](https://github.com/Homebrew/homebrew/issues/23500) I also had to do this: sudo chown -R $(whoami):admin /usr/local Because of some permission issues.