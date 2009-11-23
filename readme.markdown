Ad Hoc App Packager (adhoc) Version 1.0 by Aral Balkan
======================================================

Copyright (c) 2009 Aral Balkan ([Blog](http://aralbalkan.com), [Twitter](http://twitter.com/aral))
Released under the open source MIT License.

Packages an Ad Hoc distribution. 

Usage:
------

  1. Copy the adhoc folder into your Xcode project folder
  2. Make an Ad Hoc distribution build in Xcode
  3. Run <code>./adhoc/package [ConfigurationName]</code>

If you leave out <code>[ConfigurationName]</code>, adhoc will default to the configuration name of "Distribution" (without quotes).

Your Ad Hoc IPA file and the correct provisioning profile to send to your beta testers will be in the <em>adhoc/packages/<AppVersion>/</em> folder.

The dSYM file (which you can use to desymbolize crash reports from your beta testers) will also be backed up to the same folder. Do not send this to your beta testers. 

See: [more information on dSYM files](http://furbo.org/2008/08/08/symbolicatifination/).

Notes:
------

  * If you want a custom icon in your IPA file, create a 512x512 PNG/JPG, save it as "iTunesArtwork" (without an extension, and without the quotes), and copy it into the root folder of your project. 
