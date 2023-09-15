# clear-bash-history
clear-bash-history - easily clear all bash command history (up arrow keys), for privacy.

[![Platform: GNU/Linux](https://img.shields.io/badge/platform-GNU/Linux-blue.svg)](www.kernel.org/linux.html)

REQUIRES and DEPENDS UPON ``bash``- be sure to have it installed.

# Setup (Linux)
Append a line in your ``.bashrc``;

```nano /home/$(whoami)/.bashrc```

```alias cbh="echo 'Fully clearing bash history, then exiting...' && cat /dev/null > ~/.bash_history && history -c && history -w && exit"```

(see aliasCmd.sh if the text-formatting makes it hard to copy from here)

After that, close and re-open all of your Terminal emulators to enable the command to work inside of them.

# Setup (Haiku)
Append a line in your ``bashrc``;

```nano ~/config/settings/bashrc```

```alias cbh="echo 'Fully clearing bash history, then exiting...' && cat /dev/null > ~/.bash_history && history -c && history -w && exit"```

(see aliasCmd.sh if the text-formatting makes it hard to copy from here)

After that, close and re-open all of your Terminal emulators to enable the command to work inside of them.

# Usage
You can clear all bash command history (up arrow keys) at any time by opening a Terminal and typing the ``cbh`` command, now.


