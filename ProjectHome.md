# Media Player 2 #
This plugin was created, because of lack of possibility to show subtitles in **mediaplayer** on certain images of IPBox sh4 sattelite receivers.

Media Player source is from [Openpli project](http://openpli.org/)

If you are satisfied with this project and you would like to support me please consider donation:

<a href='https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Y4J4HAWCPTE78&lc=SK&item_name=mediaplayer2%20donation&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHosted'><img src='https://www.paypalobjects.com/en_US/ihttp://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk/btn/btn_donate_LG.gif' border='0'></img></a>

![http://mediaplayer2-for-sh4.googlecode.com/svn/trunk/images/compound_lq.jpg](http://mediaplayer2-for-sh4.googlecode.com/svn/trunk/images/compound_lq.jpg)

---


# Enhanced Movie Center with Subsupport #
Now you can try also EMC with subtitles support instead of MP2

EMC is based on latest source from https://github.com/betonme/e2openplugin-EnhancedMovieCenter + added support for subssupport

**v2 - fully updated to latest git source, added subtitles status screen on TV button
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.1_20150320_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-enhancedmoviecenter_git+935+8a5713a-r2_mips32el.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```**

**v1
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.7_20150108_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-enhancedmoviecenter_git+888+b459bbc-r1_mips32el.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```**

# Installation #

SSH/Telnet:
```
opkg remove enigma2-plugin-mediaplayer2
opkg remove enigma2-plugin-mediaplayer2ab
opkg update
```

**mp2 v0.59** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.59_20150320_all.ipk) [changelog](Changelog.md) + **subssupport v1.5.2 beta** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.2_20150407_all.ipk) [changelog](ChangelogSubsSupport.md)

  * note subssupport is for now beta version, since there are more changes and I wasn't  able to test them all
  * subssupport beta suffix will be removed, in case there will be no issues reported

**update 1**
  * updated changelog
  * **main**
    * fixed timing issue when custom subtitles fps is provided

  * **settings**
    * fixed setting entries names, adjusted skin
    * searchsettings
      * show all available search settings

  * **dvb**
    * fixed timing issue when custom subtitles fps is provided
    * fixed paused state handling
      * remain in paused state after seeking/skipping subtitles
      * pause subtitles timer when in paused state

  * **search**
    * Subssearch screen
      * fixed GS on cancelling choice dialog when downloading subtitles
      * "next to video" option is not shown in context menu when there is no video available
    * fixed subscene provider
    * added titlovi provider

**update 2**
  * **main**
    * fixed GS on opening Choose subtitles menu, when no service is available

  * **dvb**
    * attempt to fix GS on DMM(merlin 3) images
    * wait to release button on subtitles skipping
    * show status after manual seek/skip minute step back

**update 3**
  * **main**
    * updated changelog
    * look for fonts also in subdirectories
    * make sure there is "Regular" font listed - fixes [issue76](https://code.google.com/p/mediaplayer2-for-sh4/issues/detail?id=76)
    * added Ubuntu-sans font ipk in Downloads
    * use medium Ubuntu fonts for regular/italics when available

  * **dvb**
    * fixed critical error, which caused slowdown of service switching - [issue81](https://code.google.com/p/mediaplayer2-for-sh4/issues/detail?id=81)
    * fixed not showing last subtitle

  * **search**
    * fixed podnapisi
    * fixed subscene (persian/farsi lang issue, manual search)
    * Subssearch screen
      * keep the order of search langs
      * fixed some skin issues
    * Subssearch settings
      * fixed some skin issues
      * added jumping between providers and search config (yellow/pageUp/pageDown) button
      * added "Save as (fallback)" option
        * in case we have no filepath set and "Save as" is set to "video", "Save as (fallback)" option is used to determine download location
    * Searchparams screen
      * cache suggestion dialogs
    * History screen
      * change "settings" button color from green to blue

```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.2_20150407_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.59_20150320_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```

**mp2 v0.59** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.59_20150320_all.ipk) [changelog](Changelog.md) + **subssupport v1.5.1** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.1_20150320_all.ipk) [changelog](ChangelogSubsSupport.md)
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.1_20150320_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.59_20150320_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```

**mp2 v0.58** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.58_20150306_all.ipk) [changelog](Changelog.md) + **subssupport v1.5.0** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.0_20150304_all.ipk) [changelog](ChangelogSubsSupport.md)
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.5.0_20150304_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.58_20150306_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```

**mp2 v0.57** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.57_20150204_all.ipk) [changelog](Changelog.md) + **subssupport v1.4.9** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.9_20150204_all.ipk) [changelog](ChangelogSubsSupport.md)
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.9_20150126_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.57_20140905_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```


**mp2 v0.56** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.56_20140905_all.ipk) [changelog](Changelog.md) + **subssupport v1.4.8** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.8_20150126_all.ipk) [changelog](ChangelogSubsSupport.md)
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.8_20150126_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.56_20140905_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```

**mp2 v0.56** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.56_20140905_all.ipk) [changelog](Changelog.md) + **subssupport v1.4.7** [download](http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.7_20150108_all.ipk) [changelog](ChangelogSubsSupport.md)
```
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-subssupport_1.4.7_20150108_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/enigma2-plugin-extensions-mediaplayer2_0.56_20140905_all.ipk
opkg install http://dl.bintray.com/mx3l/generic/python-xmlrpc_2.7.2-r7.17_mips32el.ipk
```

[older versions](DownloadsPage.md)

**Restart Enigma2**


---


# Features #

## Media Player ##
  * added possibility to correctly display external subtitles
  * added possibility to show info from file/folder names in [CSFD plugin](http://www.cssf.cz/showthread.php?38339-Plugin-CSFD) (plugin created by petrkl12)
  * added possibility to change aspect ratio
  * added possibility to open extensions menu
  * added possibility to change media framework(eplayer3/gstreamer) when supported by **Mickey GMouse**
  * added cuesheet support for all media types

### Subtitles ###
  * support for SubRIP (.srt) subtitles (supported all tags - Ubuntu font)
  * support for MicroDVD (.sub) subtitles (supported style/color tags - Ubuntu font)
  * correct displaying of special characters (automatic encoding to utf-8)
  * dynamic change of encoding in case special characters are not shown properly
  * auto-load of supported subtitles
  * choosing size, color, font, shadow, background and position of subtitles
  * possibility to choose external subtitles from filelist
  * SD/HD skin compatible

### Subtitles search ###
  * based on [xbmc-subtitles](https://github.com/amet/script.xbmc.subtitles) project(service scripts)
    * [Titulkycom](http://www.titulky.com) (login optional)
    * [Edna.cz](http://edna.cz)
    * [SerialZone.cz](http://www.serialzone.cz)
    * [OpenSubtitles](http://opensubtitles.org)
    * [Itasa](http://www.italiansubs.net) (login neccessary)
    * [SubtitlesGR](http://www.subtitles.gr)
  * based on [podnapisi](https://github.com/amet/service.subtitles.podnapisi)
    * [Podnapisi](http://www.podnapisi.net)
  * based on [subscene](https://github.com/manacker/service.subtitles.subscene.git)
    * [Subscene](http://subscene.com)
  * based on [titlovi](https://github.com/mikimac/service.subtitles.titlovi.git)
    * [Titlovi](http://titlovi.com)


---

# Controls #
  * **ZOOM/5** - change aspect ratio
  * **RIGHT/LEFT** - increase/decrease subtitles delay
  * **INFO(I)** - when pressed in file/play list, it shows info in CSFD plugin
  * **SUBTITLES/TEXT** - shows subtitles menu
  * **TV** - refreshes subtitles position, in MP2 0.59 shows subtitles status
  * **0** - mark position
  * **NEXT(>)** - go to next mark if available/go to next item in playlist
  * **PREVIOUS(<)** - go to previous mark if available/go to previous item in playlist


---

# Customization #
  * [How to add custom colors](Colors.md)
  * [How to add custom fonts](Fonts.md)

---

# Compatibility with other platforms #
Plugin is platform independent, its completely written in python, so if you have enigma2 satellite receiver, it should work.

Tested on **sh4, mipsel** platform

---

# Localization and Encodings #
**Supported locales:**
  * english
  * slovak
  * czech (by **Vlad Kuzba**)
  * polish (by **Micky GMouse**)

**Supported encodings:**
  * Arabic
  * Greek
  * Central and Eastern European
  * Western European
  * Russian
  * Turkish

---

# Issues #
In case of any problems please fill an issue [here](http://code.google.com/p/mediaplayer2-for-sh4/issues/entry).