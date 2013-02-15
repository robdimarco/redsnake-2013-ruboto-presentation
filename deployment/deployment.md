!SLIDE commandline
# Basic Installation

    $ rake install start

!SLIDE bullets incremental
# Deployment Details

* Compile Java code
* Build APK package
* Install on emulator

!SLIDE bullets incremental
# Running on Device

* Use Ruboto Core Platform App
* OR
* Bundle JRuby jars in Package

!SLIDE commandline
# Ruby Script Update

    $ rake update_scripts

!SLIDE bullets incremental
# Physical Devices
* SD Card / USB
* Dropbox
* Github (with QR Code!)
* Google Play

!SLIDE bullets
# Ruboto IRB

* Great for learning framework
* demo-opengl.rb 
* [https://github.com/ruboto/ruboto-irb](https://github.com/ruboto/ruboto-irb)

!SLIDE bullets incremental
# Caveats

* Performance (Startup/Optimization)
* Callbacks (Java calling Ruby)
* Currently limited to Activities, BroadcastReceievers, and Services