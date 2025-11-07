# Eggdrop Service Script: `service.tcl`

**Service Bot** – modular-git BETA version. Use at your own risk: the script may contain bugs that could crash your bot or disrupt your IRC channel.

---

## Features

* Custom and random kick messages
* Basic channel moderation: kick, ban, op, deop, voice, devoice, unban, chanmodes
* Designed to manage free-op channels
* Supports mIRC color codes in messages
* Multiple bot prefixes for commands

---

## Requirements

* **`tcllib`** – required for the `inifile` package to read configuration and commands files
* **`git`** – required for update management and distribution
* **`CHANLEV +m`**

---

## Installation

1. Navigate to your Eggdrop's `scripts` directory:

```bash
cd /path/to/your/eggdrop/scripts
git clone https://github.com/r0t3n/service.git
cd service
```

2. **Configuration**
   Some settings are read from `.conf` and some from `.ini`. Update both until the `.conf` is fully phased out:

* Edit `service.conf`
* Edit `service.ini`, changing `homechan`, `adminchan`, and `helpchan` values

> Minimal setup is sufficient. You can change default kick messages, but avoid modifying other settings, **especially the `chanflags` array**.

3. **Load the script in your Eggdrop**
   Add the following line to your Eggdrop configuration file:

```tcl
source scripts/service/service.tcl
```

Then rehash your bot (if already running) or start the bot.

---

## Upgrade

To update the script:

```bash
cd /path/to/your/eggdrop/scripts/service
git pull
```

After pulling, rehash your Eggdrop to apply the latest updates.

---

## Errors

Please report bugs with as much detail as possible. The output from `errorInfo` will be very helpful.

* [Issue Tracker](https://github.com/norrchr/issues)

---

## Help

* Contact `r0t3n` via Quakenet’s channel: `#r0t3n`
* More details: [Service Wiki](https://github.com/norrchr/service/wiki)
* For bugs or general questions: [open an issue](https://github.com/norrchr/issues) or contact on [IRC](https://webchat.quakenet.org/?channels=#r0t3n)

---

## Feature Requests

* Via [IRC](http://webchat.quakenet.org/?channels=#r0t3n)
* Or add a request on the [issue tracker](https://github.com/norrchr/issues)
