## All pulls are currently handled via QuickBox own GitLab at [github.com](https://github.com)

## Script status

[![Version 2.4.8-production](https://img.shields.io/badge/version-2.4.8-674172.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31) [![GNU v3.0 License](https://img.shields.io/badge/license-GNU%20v3.0%20License-blue.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31)

#### Ubuntu Builds
 [![Ubuntu 15.10 Passing](https://img.shields.io/badge/Ubuntu%2015.10-passing-brightgreen.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31) [![Ubuntu 16.04 Passing](https://img.shields.io/badge/Ubuntu%2016.04-passing-brightgreen.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31) [![Ubuntu 16.10 Passing](https://img.shields.io/badge/Ubuntu%2016.10-passing-brightgreen.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31)

#### Debian Builds
[![Debian 8 Passing](https://img.shields.io/badge/Debain%208-passing-brightgreen.svg?style=flat-square)](https://plaza.quickbox.io/t/quickbox-readme-md/31)

---

###Quick Advisory Notice(s) on QuickBox

>### :rotating_light: OVH DEFAULT KERNEL NOTICE!
grsec is built into OVH's custom kernel and it absolutely wrecks havoc when using these panels where we depend on the ability for one user (www-data) to see the processes of another running user ($username).
<br/>This can be seen clearly by using a task manager such as h/top.
<br/>With grsec enabled you can only see the processes owned by your user unless you run htop as root. As such, it is highly recommended to use the stock kernel for your distribution or at the very least installing an OVH kernel that is not compiled with grsec
<br/>If you are using So You Start (SYS) as a host, you should opt to use the distribution kernel. You will see this as a checkbox option when installing your server. Otherwise, QuickBox will handle this for you on install.



---
> Please understand that we do not want to push this project as a means to supply a commercially used product, ie; seedbox provider - so keep this in mind - only if you wish to sale slots on your server. Though it is very multi-user friendly... it is also not free of it's faults due to it's high amount of capabilities and being publicly available. This is a community based project that is a measure of goodwill to be given to such an outspoken and freethinking community.

### A Preview of Quick Box
https://quickbox.io/video/quickbox-video-demo-tour.mp4

---

This script has the following features

* A multi-user environment, complete with scripts to add and delete users.
* Linux Quota, to control how much space every user can use in the box. This can be controlled via the '__setdisk__' command.
* Customized Seedbox Dashboard located at https://SERVER_IP/
* HTTPs Downloads directory (https://SERVER_IP/${username}.downloads)
* Obscures ports for ssh and ftp. __SSH = 4747__ | __FTP = 5757__ (note, this is not for security reasons... it's simply a means to reduce bad bot hits from all over the web)
* Creates a limited shell access environment. This gives your additional created users the ability to interact with their seedbox via ssh on port 4747 w/o having access to other users shells and/or root/sudo commands and functions.

## Installed software
* Linux Quota
* LShell - (LimitedShell for additional users to ssh)
* SSH Server (for SSH terminal and sFTP connections)
* pureftp - vsftp (CuteFTP multi-segmented download friendly)
* HTTPS - Web Console
* ruTorrent 3.7 + official plugins
* rTorrent 0.9.6
* libTorrrent 0.13.6
* mktorrent
* Deluge (Web-client and thin-client)
* IRSSI
* BTSync
* CouchPotato
* ConfigServer Firewall
* Emby
* Jackett
* NextCloud
* OpenVPN
* Plex
* PlexPy
* Plex Requests (.NET)
* pyLoad
* Quassel
* Quotas
* Rapidleech
* SABnzbd
* SickRage
* Sonarr
* Subsonic
* Syncthing
* X2Go - Remote Desktop
* ZNC
* .. more to come (or how about that feature request?)

## Main ruTorrent plugins
autotools, cpuload, quotaspace, erasedata, extratio, extsearch, feeds, filedrop, filemanager, geoip, history, logoff, mediainfo, mediastream, ratiocolor, rss, scheduler, screenshots, theme, trafic and unpack

## Additional ruTorrent plugins
* Autodl-IRSSI (with an updated list of trackers)
* A modified version of Diskpace to support quota (by Notos)
* Filemanager (modified to handle rar, zip, unzip, tar and bzip)
* Fileshare Plugin (http://forums.rutorrent.org/index.php?topic=705.0)
* Logoff
* Theme: QuickBox ``Dark rutorrent skin``
* Colorful Ratios: Customized to match QuickBox Theme
* __rutorrentMobile__: Mobile version of ruTorrent - seriously - toss TransDroid and the pain that it is... this is a new essential plugin (IMO)

## Before installation
You need to have a Fresh "blank" server installation.
After that access your box using a SSH client, like PuTTY.

---

## How to install

####You must be logged in as root to run this installation.


---

### Ubuntu 15.10, 16.04 & 16.10 || Debian 8

**Run the following command to grab our latest stable release ...**
```
apt-get -yqq update; apt-get -yqq upgrade; apt-get -yqq install git lsb-release; \
git clone --recursive https://github.com/QuickBox/QuickBox /root/QuickBox &&
bash /root/QuickBox/setup/quickbox-setup
```


---


## Commands
After installing you will have access to the following commands to be used directly in terminal

* <del>quickbox</del> - tells you which version QuickBox you are running and shows commands list ``deprecated due to versioning now shows on the dashboard under username dropdown as well as login to bash``
* __createSeedboxUser__ - creates a shelled seedbox user
* __deleteSeedboxUser__ - deletes a created seedbox user and their directories
<sup>**This is permanent, current data will be deleted - you can create them again at any time**</sup>
* __changeUserpass__ - change users SSH/FTP/deluge/ruTorrent password
* __setdisk__ - set your disk quota for any given user
* __showspace__ - shows amount of space used by each user
* __reload__ - restarts your seedbox services, i.e; rtorrent & irssi
* __upgradeBTSync__ - upgrades btsync when new version is available
* __upgradePlex__ - upgrades Plex when new version is available
* __removepackage-cron__ - upgrades your system to make use of systemd
 <sup> + (must be on Ubuntu 15.10+ or Debian 8)</sup>
* __clean_mem__ - flushes servers physical memory cache (helps avoid swap overflow)


<br/>

---
## QuickBox Repo Structure
The following is the Repo structure of the current QuickBox EcoSystem. Any pull requests must be done within the repo you aim to add functionality and address any issues found.

QuickBox is divided into it's relevant parts that aim to make the update process as simple as possible on a rolling update fashion. This is so we can continually pull fresh commits/updates as they are released within the master branch of each designated zone. Sounds technical? It's actually simple... it works by cloning certain parts of QuickBox into relevant pieces on your server for ease of use and updates.

#### Here are the Repos & examples:

* [quickbox_setup](https://github.com/QuickBox/quickbox_setup) - this is the repo used for the initial setup of QuickBox on the users server. This can be installed by doing the following:
 ```
git clone https://github.com/QuickBox/quickbox_setup quickbox_setup
cd quickbox_setup
bash quickbox-setup
 ```

* [quickbox_rutorrent](https://github.com/QuickBox/quickbox_rutorrent) - this is the repo used for ruTorrent. All ruTorrent relevant plugins and theme adjustments, fixes, additions and extra enhancements will be included here.
Much like the quickbox_setup repo, the script will be pulled via the following:
```
git clone https://github.com/QuickBox/quickbox_rutorrent quickbox_rutorrent
```
This is handled during the initial install with the quickbox_setup repo. The quickbox_rutorrent directory is then copied over to your /srv/ directory where it maintains it's git-like qualities for easy updating later on.

* [quickbox_dashboard](https://github.com/QuickBox/quickbox_dashboard) - this is the repo used for the QuickBox UI. All QuickBox Dashboard relevant widgets and theme adjustments, fixes, additions, extra enhancements and **future language files** will be included here.
Much like the other repo's, the script will be pulled via the following as an example:
 ```
git clone https://github.com/QuickBox/quickbox_dashboard quickbox_dashboard
cd  quickbox_dashboard
mkdir -p /srv/rutorrent/home
cp -r home/. /srv/rutorrent/home
 ```
<sup>Again, this is just an excerpt and this function is handled by the script. Just as with any of the other features, navigate to ``/srv/rutorrent/home`` and run ``git pull`` to push updates to your server.</sup>

* [quickbox_packages](https://github.com/QuickBox/quickbox_packages) - this is the repo used for the installers and uninstallers. All needed files/commands for packages installers/removers as well as plugin installers/removers will be included here.
Much like the other repo, the script will be pulled via the following:
 ```
git clone https://github.com/QuickBox/quickbox_packages quickbox_packages
cd  quickbox_packages
cp -r quickbox_packages/. /usr/local/bin/
 ```
<sup>Again, this is just an excerpt and this function is handled by the script. Just as with any of the other features, navigate to ``/usr/local/bin/quickbox`` and run ``git pull`` to push updates to your server.</sup>

* [club-Swizards](https://github.com/Swizards/club-Swizards) - this is the custom ruTorrent theme created and designed by Swizards. Any adjustments you would like to push can be made here. Updating the template... again, as simple as ``git pull`` from within ``/srv/rutorrent/plugins/theme/themes/club-Swizards``. The theme is independent of the update for the rutorrent directory which handles plugins etc.
