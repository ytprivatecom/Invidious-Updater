# Invidious-Updater

## Script to update [Invidious](https://github.com/omarroth/invidious) git repository

* Automatically update git repo, rebuild and restart service

## Screenshot
![screenshot](https://raw.githubusercontent.com/tmiland/Invidious-Updater/master/img/Screenshot%20at%2011-31-38.png)

## Installation

download and execute the script :
```bash
wget https://github.com/tmiland/Invidious-Updater/raw/master/invidious_update.sh
chmod +x invidious_update.sh
./invidious_update.sh
```

## Usage
1. Update Invidious
  1. No arguments (Default) Will use branch "Master" and prompt user for each step.
  1. -f FORCE YES (Force yes, update, rebuild and restart Invidious)
  1. -p Prune remote. (Deletes all stale remote-tracking branches)
  1. -l Latest release. (Fetch latest release from remote repo.)

2. Update the Script
  2. Downloads and executes the script from this repo.

3. Install Invidious service for Systemd
  3. 
  
4. Install invidious
   4. Add invidious user and clone repository [y/n]
   4. Setup PostgresSQL [y/n]
   4. Setup Invidious [y/n]
   4. Setup Systemd Service [y/n]

5. Exit
  5. Exits the script

## Testing
- [x] Tested extensively on Debian 9

## Todo
- [ ] Rewrite the update procedure 
- [ ] Add database maintenance option [Database Information and Maintenance](https://github.com/omarroth/invidious/wiki/Database-Information-and-Maintenance)
- [ ] Add option to compile imagemagick from source [Issues with Captcha on Debian and Ubuntu](https://github.com/omarroth/invidious/wiki/Issues-with-Captcha-on-Debian-and-Ubuntu)

## Compatibility and Requirements
* Debian 8 and later
* Ubuntu 16.04 and later

## Credits
- Code is mixed and and customized from these sources:
  * [Invidious](https://github.com/omarroth/invidious#linux)
  * [nginx-autoinstall](https://github.com/angristan/nginx-autoinstall)
  * [Git-Repo-Update](https://github.com/KillianKemps/Git-Repo-Update)
  * [ghacks user.js updater.sh](https://github.com/ghacksuserjs/ghacks-user.js/blob/master/updater.sh)
