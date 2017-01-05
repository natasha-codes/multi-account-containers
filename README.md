# Containers: Test Pilot Experiment

Soon to be [![Available on Test Pilot](https://img.shields.io/badge/available_on-Test_Pilot-0996F8.svg)](https://testpilot.firefox.com/)

[Embedded Web Extension](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/Embedded_WebExtensions) to experiment with [Containers](https://blog.mozilla.org/tanvi/2016/06/16/contextual-identities-on-the-web/) in [Firefox Test Pilot](https://testpilot.firefox.com/) to learn:

* Will a general Firefox audience understand the Containers feature?
* Is the UI as currently implemented in Nightly clear or discoverable?

See [the Product Hypothesis Document for more
details](https://docs.google.com/document/d/1WQdHTVXROk7dYkSFluc6_hS44tqZjIrG9I-uPyzevE8/edit?ts=5824ba12#).


## Requirements

* node 7+ (for jpm)
* Firefox 52+ (For now; aiming at Firefox 51+)


## Run it

See Development


## Development
### Development Environment

Add-on development is better with [a particular  environment](https://developer.mozilla.org/en-US/Add-ons/Setting_up_extension_development_environment). One simple way to get that environment set up is to install the [DevPrefs add-on](https://addons.mozilla.org/en-US/firefox/addon/devprefs/). You can make a custom Firefox profile that includes the DevPrefs add-on, and use that profile when you run the code in this repository. 

1. Make a new profile by running `/path/to/firefox -P`, which launches the profile editor. "Create Profile" -- name it whatever you wish (e.g. 'addon_dev') and store it in the default location. It's probably best to deselect the option to "Use without asking," since you probably don't want to use this as your default profile.

2. Once you've created your profile, click "Start Firefox". A new instance of Firefox should launch. Go to Tools->Add-ons and search for "DevPrefs". Install it. Quit Firefox.

3. Now you have a new, vanilla Firefox profile with the DevPrefs add-on installed. You can use your new profile with the code in _this_ repository like so:


### Run with jpm

1. `git clone git@github.com:mozilla/testpilot-containers.git`
2. `cd testpilot-containers`
3. `npm install`
4. `./node_modules/.bin/jpm run -p /Path/To/Firefox/Profiles/{junk}.addon_dev -b FirefoxDeveloperEdition`

Check out the [Browser Toolbox](https://developer.mozilla.org/en-US/docs/Tools/Browser_Toolbox) for more information about debugging add-on code.


### Testing
TBD


### Distributing
TBD
