## ABOUT ME

Just some dude trying to develop stuff. Mostly Debian and Virtualization
related.

## DEBIAN REPO

Most of my GitHub projects have a Debian package that can be found on my own
repo, hosted on my private website https://muspekaren.se/ .  
First time users should set up a Debian 11 VM that is connected to the
internet.  
Run the command below to add the repo to your Debian 11 machine.

```
DIR=$(pwd) && cd /tmp &&
wget https://raw.githubusercontent.com/ServerMonkey/servermonkeys-devtools/main/bin/add-repo_servermonkey \
-qO add-repo_servermonkey &&
echo "e5b0c63911840ca80d0db84b03f4ed7ea49c396bcd9b92fc53f7b3ea42b78d90 add-repo_servermonkey" |
sha256sum -c && sudo sh add-repo_servermonkey ; rm -f /tmp/add-repo_servermonkey ; cd "$DIR"
```

To understand what this script is doing read the code here:
[ServerMonkey/servermonkeys-devtools](https://github.com/ServerMonkey/servermonkeys-devtools/blob/main/bin/add-repo_servermonkey)

This repo is currently in BETA. There are no stable releases, only development
builds.  
With that said all packages should still be usable.  
Please report all bugs to me here on GitHub.
