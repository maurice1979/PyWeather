# PyWeather changelog

Quick note: While in beta, commits are not counted as versions. When I decide to push a release, I push a release. There will also be a running changelog for the in-development version, so I'm not remembering every single change I made in the version.


## version 0.3.1 beta (The Updater Update) - To be released
* Adds an updater to PyWeather to check for the latest updates, and download them
* Revamps the extra options selection screen
* The dew point is now shown on the summary screen
* PyWeather has a double redundancy geolocator situation, Google first, Nominatim second, then a fail if nothing returns.
* Setup script checks for a connection to Google/Nominatim, and for the shutil library

## version 0.3.0 beta (The Setup Update) - Released 2/26/2017
* Adds a setup script that guides new users through the setup process
* Switches the geolocator from Nominatim to Google's geolocator (experimental)

## version 0.2.3 beta (The Bug Snatching Update) - Released 2/24/2017
* Fixes a bug in which detailed hourly data wouldn't show without turning verbosity on
* Fixes a bug in which the temp in detailed hourly data wouldn't iterate properly
* Fixes a bug in which PyWeather didn't stop at 30 iterations of detailed hourly data
* Fixes a semi-bug in which PyWeather wouldn't properly handle a missing API key

## version 0.2.2 beta (The Pressure Update) - Released 2/22/2017
* Adds current/pressure data to the current screen
* Fixes a bug in which users in the UK would see their 1 hour precip as -9999 in/-- cm (now corrects to 0.0 in/cm)

## version 0.2.1 beta (The Verbosity Update) - Released 2/22/2017
* Adds verbosity to newer functions of PyWeather. PyWeather loves verbosity.
* Replaces double verbosity with jsonVerbosity, as to not confuse people.
* Adds a check for snow data. We made sure people living near the equator don't feel sad when "Snow data" is always 0.0 inches.
* The loading bars are now turned off when verbosity is enabled.
* PyWeather can now accept numbers as inputs for different functions, to make life a little easier.
* Fixes some other issues.

## version 0.2 beta (The Initial Update) - Released 2/22/2017
* Initial build