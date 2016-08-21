---

##CHANGELOG v2.4.6:
_Changelog updated Saturday, August 21, 2016_

---

###General adjustments & additions
* Version Bump set to **2.4.6**
* Below we will outline the changes that have brought us from 2.4.0 to the current stable 2.4.4

###Commit Histories by Submodule v2.4.6
---

####QuickBox/quickbox_dashboard version 2.4.6

* [fix] deluge & rutorrent panel links [633446c2](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/633446c2c7508d5946380f39bc4a11150c1eae3a)
* [enhancement] nextcloud is here! [13c75b70](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/13c75b7084b783bc3b9e0c67c3df00127a905b47)
* [fix] set a minimum of '0' on bandwidth chart to avoid negative values [66e4f0aa](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/66e4f0aac1455455d9427636e53ce34fa73aa10d)
* danish language file updated with new values [346d1f81](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/346d1f8120a4e7d1ee9f823efe9bb78509ae5e16)
* [ux] a more lean and accurate cpu widget [c6d50168](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/c6d50168e38bd04e22fccb7b5b0338e02679c423)
* update on language files [152c268b](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/152c268b012ab464f6eb7d9edad205a98c06be80)
* [fix] removed characters causing breakage on language files [66264062](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/66264062123399345ef68d3dfba20118fb0b4600)


####QuickBox/quickbox-packages version 2.4.6

* Further refine IFACE detection X2 [f607391b](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/f607391b92cf0f3239b4a1d87c64887dd81080ef) & [6e42136f](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/6e42136fc2dbcffe569683dce62287140fd5c9bd)
* [security] Remove php execution for existing users on update [1d74f999](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/1d74f99974231955cac6b00d2715fa2e151737e0)
* [fix] Spinner causes breakage on interactive scripts [888be134](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/888be1349f989c6e9af03da10700f11ca2c3a914)
* cleanup on system installer packages [a0f12fc1](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/a0f12fc15b2b0a7d21adb2da2a1a5660857996e8)
* [enhancement] nextcloud is here! [7c93e13c](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/7c93e13c6e8890301846782c3d8d43b9a2d8c12f)
* [fix] update the csf archive download link to their new release location [e9074ce6](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/e9074ce6700b500ed0c1440c1d822a678ae09be8)
* Upgrade box to newest version [520b1893](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/520b1893465a621b4d2cc4699e62490d24daa443)
* remove old .startup remnants on sonarr package [35e44e5d](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/35e44e5db4a4b4260f3198b4b7ba7e3de9ff8cb2)
* restart apache after openvpn installation [a498feca](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/a498feca5e26ef74a3072c25a1bece145f1435a1)
* remove organize user home directory function [c84b2186](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/c84b2186777c9906defdf934bb9bb2ba7a3c18a1)
* [security] require a valid user to access vpn configs [a421c585](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/a421c585b7e5bda1c3f7a55c18c3d62f070cee57)
* [enhancement] vpn management now included - type: `quickVPN` [c5dbf75a](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/c5dbf75a1ffc9eed4878240eecc7189b7dcfdc5d)


####QuickBox/quickbox-rutorrent version 2.4.5

* updated gitignore - overlook conf and share directories [69aa9c50](https://lab.quickbox.io/QuickBox/quickbox_rutorrent/commit/69aa9c5079fc7bfe04ed4a195ded682ceed0c0d9)
* update rutorrent to latest novik/master [14d8951a](https://lab.quickbox.io/QuickBox/quickbox_rutorrent/commit/14d8951ac669fe92fbdfb221e39d6fe24f66d22b)


####QuickBox/quickbox_rutorrent-plugins version 2.4.5

* No Changes


####QuickBox/quickbox-setup version 2.4.5

* Further refine IFACE detection [96553245](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/96553245c90e089b7f4720db9aa170556cf36f39)
* minor typo fix [d634ec68](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/d634ec682d13f8d49912af39c7cb4079a1ff1065)
* Version bump deluge libtorrent to 1.1.1 [5a16e32b](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/5a16e32bd5fdacb24d2c70ea1a43b74b5315e565)
* [enhancement] Expand upgradeDeluge to allow upgrading libtorrent and deluge through recompiling [325018ec](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/325018ec12075e67ad483531a21a985306e49fd6)
* [security] Disallow php execution from rtorrent/deluge apache servers X2 [3892b6d7](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/3892b6d7ed6284f63dff450a468623dca12ceba6) & [6d3df8d8](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/6d3df8d84e6edc598243841f1631670f9bd03eb2)
* Remove deprecated webconsle code from changeUserpass [3df0ef7c](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/3df0ef7cbb562ff8773ba6d9d4e47b0c4726911f)
* Make /install dir if 10g=yes [9bf4f74e](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/9bf4f74e095961939ac922594a289ab04a05d1ad)
* Apache doesn't need sudo pkill or sudo killall anymore [d88ea63b](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/d88ea63b2c8666c17b185e99a4971034c3d35481)
* Better `fixhome` command [b085d804](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/b085d804cbcbd73fd803e33ee2717de960abea46)
* Setup now checks if a grsec kernel is present and fails if the user declines to upgrade [2b27087c](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/2b27087c99ac7136972c4ac46e381fdaebe52d5a)



---

##CHANGELOG v2.4.5:
_Changelog updated Saturday, August 21, 2016_

---


###General adjustments & additions
* Version Bump set to **2.4.5**
* Below we will outline the changes that have brought us from 2.4.0 to the current stable 2.4.4

###Commit Histories by Submodule v2.4.5
---

####QuickBox/quickbox_dashboard version 2.4.5

* updated language files to reflect new batch installer command `box install <app>` [4f7565b0](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/4f7565b0d5735d278d49d0cb12dff629d8611c66)
 <sup>+ BOX is QuickBoxs new batch installer for easy installation of applications simultaneously. Type `box install <app>` to install an application from cli or type: `box install <app> <app>` to install multiple applications at once.</sup>
* minor adjustments... _file: lang_fr_ [a399dbc7](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/a399dbc79d4fede615bae6659700dc5ef74447c7)
* Translation added for 'select language' + minor changes. [4113237b](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/4113237b692cdfc3516fa2222b74308fd0fd199d)
* we only need to log errors from the dashboard [4e649551](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/4e649551aa5319cb0fbe091eb84a42e7daf7f9ed)
* added additional value to language files - 'Select Language' [472ae6fd](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/472ae6fdafaa6de12a0a1c1617bc6508a634df07)
* address minor whitespacing [e9cb6383](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/e9cb6383f3829d1dcec060b6877577474ef3dd31)
* **[fix]** addressed missing opening php operator [2e5ac300](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/2e5ac300fff0d6e825edfd55059bd2934e93fe84)
* Add translations for CLI and OpenVPN package + quickVPN command [cc295426](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/cc2954260b05aa8bc65aa506517f5bd54287c942)
* better openvpn info and integration within dashboard [95c04757](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/95c04757113839a57b3ba7e7f15a5a98f8ff02a7)
* **[ux]** minor dashboard aesthetics [9375d909](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/9375d9090e1aae22e24bcdc436099bba0cdafb71)
* add openvpn config file download to 'Downloads' Menu if installed per user [9c0baa3a](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/9c0baa3a6b6b257c3bafd8ec81f6d3d122a1df99)
* **[enhancement]** better approximation of bandwidth chart values [1992369c](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/1992369caafeb1c36a629fdb83cd5cec424c39a4)
* **[fix]** addressed issue with disk percentage calculations on certain environments [56163af6](https://lab.quickbox.io/QuickBox/quickbox_dashboard/commit/56163af66b45c1bf1096560bbcdbcf48134b4e41)
 <sup>+ special thanks to @sadpanda for granting access to a machine to troubleshoot and find a fix for this</sup>


####QuickBox/quickbox-packages version 2.4.5

* New method for determining IFACE, more OpenVZ-friendly [d539c3b5](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/d539c3b5092d3c19972e7a57fff1fe7c453595ba)
* Remove outdated and refactored QBPM [d0c171dd](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/d0c171dd0afbe0d6c164d37cd24bad5a04068c71)
* Introducing box -- QBPM just got better! [d4e0a24b](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/d4e0a24badd14cada54a1ffe70e0e45dc9a78631)
* updated installer packages for cleaner and quieter execution [6e29dd38](https://lab.quickbox.io/QuickBox/quickbox_packages/commit/6e29dd38f02403e6efa3db86c89a4b7bf6e1a58f)

#####What is `box`?
Building off of our CLI based updater, there have been a few tweaks to make installing and/or removing multiple applications at once a total breeze. Additionally, the new QBPM (QuickBox Package Management) codenamed: BOX now supports updating/upgrading your QuickBox. It's truly an all-in-one management utility for those of us who prefer rolling in ssh.
If you prefer to still use the GUI aspect of the installer you can call box without any arguments. box -h will show you a help screen.
**BOX CHEATSHEET**
```
# box -h
Usage: box [ install | remove | list | update ] pkg

Note: Only install and remove functions accept package arguments. List
   and update must be run without modifiers



install        The install function requires at least one package
               name as an argument but will accept multiples

               Example: box install quassel syncthing znc

remove         The remove function requires at least one package
               name as an argument but will accept multiples

               Example: box remove quassel syncthing znc

update         The update command will update your local QuickBox
               repository to the latest version

list           The list command will list packages available to be
               managed by box

```


####QuickBox/quickbox-rutorrent version 2.4.5

* No Changes


####QuickBox/quickbox_rutorrent-plugins version 2.4.5

* .gitignore added - ignore plugins conf.php [88355fa9](https://lab.quickbox.io/QuickBox/quickbox_rutorrent-plugins/commit/88355fa9ebba7e6adea571e555f80c2455fc83ab)
* update rutorrent plugins to latest novik/master (fix utf8 encodings) [c3c0c5c4](https://lab.quickbox.io/QuickBox/quickbox_rutorrent-plugins/commit/c3c0c5c4d9566538c6498a9d2cbba097ee70f936)


####QuickBox/quickbox-setup version 2.4.5

* added newer archived source of plex [2c561819](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/2c5618197c4a8bc48ae972ee20ba877190380309)
* **[enhancement]** new aliases for added for easy disk widget fixes/updates [cbcd144f](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/cbcd144fdffb072f780ec65970fa7d038df47782)
 <sup>+ `fix-disk_widget_home` - easily copy over updated/default disk widget from local repository to your dashboard, home mounted installs only</sup>
* **[fix]** 10g function defaults addressed [042d1a6a](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/042d1a6a75ca75b02cc6f67dab72016abdc537e9)
* quickVPN added to sudoers allowed aliases [70f3c926](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/70f3c9262ffa27d5ddbeee38c805f8a8dbd5dc82)
* Remove old cron function from running [23ed699a](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/23ed699a74d6d629d58f4f847c25fef272cef2cc)
* New method for determining IFACE, more OpenVZ-friendly [a1aee6ca](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/a1aee6ca0c698a028b57216381d39773b577592a)
* **[enhancement]** ffmpeg on script install now includes x265 libraries on build [5ea7358f](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/5ea7358f20722015a1163b2494f8a555cfe71536)
* 10G inclusion and deluge password changing improved [9ec8b7ae](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/9ec8b7ae118ab4323fd24b6c259385cd3bbf1109)
* **[enhancement]** 10G function added to setup script [886d3ff5](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/886d3ff5380a0d802b53b325b3850c32c3638688)
* allow `install_ffmpeg` to be fired as system command [79a62e8a](https://lab.quickbox.io/QuickBox/quickbox_setup/commit/79a62e8a540dcad21efbc930179312ab25357d21)
