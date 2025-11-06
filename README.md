# eggdrop service script: service.tcl
Service modular-git BETA version, use at your own risk, script may contain bugs which may crash your bot, or totally bork your IRC channel.

# Requirements:

tcllib - required for the inifile package to read the config and commands file

git - required for update management and distribution

# Installation:

cd to your eggdrop's scripts directory, and type: git clone https://github.com/r0t3n/service.git

cd service

*** Some settings are read from the .conf and some from the .ini, best to update both until the .conf is fully phased out

edit service.conf

edit service.ini, changing the homechan/adminchan/helpchan values

This is the minimal setup. You may go through and change the default kickmsg values, but generally don't touch anything else, especially the chanflags array.

Edit your eggdrops config file, and add `source scripts/service/service.tcl` to the end of it. If the bot is loaded, rehash it; otherwise, start your bot.

# Upgrade:

cd to scripts/service/ and type `git pull`

This will download all the latest script updates, then rehash your eggdrop.

# Errors:

Please post a bug report, including as much information as possible, to the issue tracker. The errorInfo output will be helpful. 

# Help:

Contact r0t3n via quakenet.org channel #r0t3n
More details on the [wiki](https://github.com/someuser/service/wiki).

Webchat: http://webchat.quakenet.org/?channels=#r0t3n

# Feature requests

Contact via IRC or add a feature request to the issue tracker
