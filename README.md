<img src="logo.png" align="right" />

# QtFirebase
An effort to bring the Firebase C++ API to Qt 5

QtFirebase aim to bring all the features of the Firebase C++ SDK to Qt 5 - both as C++ wrappers and as QML components.

Please bear in mind that the Firebase C++ SDK currently only support the mobile platforms Android and iOS.

You can still build QtFirebase on other platforms as the project provide "empty shells" or placeholder components - they just return default/empty values when used. Because of this you won't see e.g. ads from AdMob in your desktop builds.

This is due to Google's own limitations in the Firebase C++ SDK implementation.

# Features / Status
The following [features](https://firebase.google.com/docs/cpp/setup) have a working Qt 5 C++ and QML counterpart

Feature | Library | C++ | QML | Credits
------- | ------- | --- | --- | -------
Base                      |libapp.a             |✓|✓|[Lars Pontoppidan](https://github.com/Larpon)
AdMob                     |libadmob.a           |✓|✓|[Lars Pontoppidan](https://github.com/Larpon)
Analytics                 |libanalytics.a       |✓|✓|[Lars Pontoppidan](https://github.com/Larpon)
~~Authentication~~	          |~~libauth.a~~          |in progress |:wrench: |[Isy](https://github.com/isipisi281)
~~Realtime Database~~	        |~~libdatabase.a~~      |in progress |:wrench: |[greenfield932](https://github.com/greenfield932)
~~Invites and Dynamic Links~~	|~~libinvites.a~~       | | |
Cloud Messaging	          |libmessaging.a     |✓|✓|[Isy](https://github.com/isipisi281)
Remote Config             |libremote_config.a   |✓|✓|[greenfield932](https://github.com/greenfield932)
~~Storage~~	                  |~~libstorage.a~~       | | |

## Contributors
With out these good people this project would not exist.

[Lars Pontoppidan](https://github.com/Larpon) (Maintainer, project founder),
[greenfield932](https://github.com/greenfield932) (Remote Config, Misc.),
[Isy](https://github.com/isipisi281) (Cloud Messaging, Misc.),
[Andrew Dolby (adolby)](https://github.com/adolby) (Cloud Messaging, Misc.), 
[li3p](https://github.com/li3p) (Misc.),


Tested Firebase C++ SDK versions:

**Base, AdMob, Analytics**
Up until commit [cb52be83](https://github.com/Larpon/QtFirebase/commit/cb52be8328a063956c2d2139fa9ab7152d955cc2)
* v2.1.0
* v2.1.1
* v2.1.2

**Base, AdMob, Analytics, RemoteConfig**
* v3.1.0
* v4.0.1

We recommend you build against the latest version of the Firebase C++ SDK.

## Stability
The Firebase C++ SDK has a lot of stability issues - which QtFirebase does it's best to work around by wrapping the API into more Qt/C++ friendly classes that prevent some of the bugs and crashes found so far.
Please use the latest SDK version to get the latest fixes.

# Setup
For a working and up-to-date example please follow the **Quick start** section found in the [QtFirebaseExample](https://github.com/Larpon/QtFirebaseExample) README.

Please see [SETUP.md](https://github.com/Larpon/QtFirebase/blob/master/SETUP.md) for instructions on how to setup QtFirebase in your QtCreator project.

# Examples
Please look at the [QtFirebaseExample](https://github.com/Larpon/QtFirebaseExample) repository.
In [SETUP.md](https://github.com/Larpon/QtFirebase/blob/master/SETUP.md) you will find details on what to add to your different project files (gradle.build, Info.plist etc.)

# Documentation
Under heavy construction.

# Support
Possible ways of getting support
* Open an [issue](https://github.com/Larpon/QtFirebase/issues)

Possible ways of giving support
* Comment helpfully on issues
* Fork, Change, Make Pull Request
* Share online
* [Buy QtFirebase &#10084;'s](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4DHVNRBQRRU96)
  You'll get a personal email full of hearts from [Black Grain](http://blackgrain.dk/games/)!

# In the wild
The following is a list of software that uses QtFirebase
* [Hammer Bees](http://blackgrain.dk/games/hammerbees/) (Casual game, [Android](https://play.google.com/store/apps/details?id=com.bitkompot.android.hammerbees.ad), [iOS](https://itunes.apple.com/us/app/hammer-bees-free/id1164069527?ls=1&mt=8))
* [Dead Ascend](http://blackgrain.dk/games/deadascend/) (Open Source, Adventure game, [Android](https://play.google.com/store/apps/details?id=com.blackgrain.android.deadascend.ad), [iOS](https://itunes.apple.com/us/app/dead-ascend/id1197443665?ls=1&mt=8))
* \<your awesome project\>
