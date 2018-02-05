+ACM- How to build this client for Debian / Ubuntu

  - +ACoAKgBb-Debian 7.X Wheezy+AF0AKgAq- Ensure that aptitude is using the backport packages by adding this line into +AGA-/etc/apt/sources.list+AGA- if it isn't already there:

    +AGAAYABg-
    +ACQAPg- deb http://http.debian.net/debian wheezy-backports main
    +AGAAYABg-

  - Install the dependencies

    +AGAAYABg-
    +ACQAPg- sudo apt-get install g make libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-thread-dev libdbdev libssl-dev libqrencode-dev libpng-dev qt5-default qttools5-dev-tools pkg-config
    +AGAAYABg-

  - Build the binaries by going into the repository's +AGA-src+AGA- directory and running:

    +AGAAYABg-
    +ACQAPg- make -f Makefile.unix
    +AGAAYABg-

    Or, if you wish to build the Qt client:

    +AGAAYABg-
    +ACQAPg- make -f Makefile.unix EmollientCoin-qt
    +AGAAYABg-

    Or, if you wish to build everything:

    +AGAAYABg-
    +ACQAPg- make -f Makefile.unix all
    +AGAAYABg-
