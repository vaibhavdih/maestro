#Changelog

## 1.0.0 - 2022-07-20

* Initial Maestro release (formerly known as Conductor)

## 1.1.0 - 2022-07-28

* `launchApp` command now can optionally clear app state
* `config` command to allow Orchestra consumers a higher degree of customization
* Fixed a bug where `ElementNotFound` hierarchy field was not declared as public

## 1.2.0 - 2022-08-04

* Config is now defined via a document separator
* launchApp no longer requires and appId
* initFlow config implemented

## 1.2.1 - 2022-08-04

* Update `YamlCommandReader` to accept Paths instead of Files to support zip Filesystems

## 1.2.2 - 2022-08-08

* Update `Orchestra` to support state restoration

## 1.2.3 - 2022-08-15

* Added support of iOS state restoration
* Exposing `appId` field as part of `MaestroConfig`

## 1.2.4 - 2022-08-17

* Add support for cli to specify what platform, host and port to connect to

## 1.2.6 - 2022-08-18

* Fail launching an iOS app if the app is already running

## 1.3.1 - 2022-08-19

* Added support for externally supplied parameters
* Added `openLink` command

## 1.3.2 - 2022-08-22

* Fix: env parameters did not work with init flows when using `Maestro` programmatically

## 1.3.3 - 2022-08-23

* Fix: iOS accessibility was not propagated to Maestro

## 1.3.6 - 2022-08-25

* Added `longPressOn` command
* Decreased wait time in apps that have a screen overlay
* Fixed CLI issue where status updates would not propagate correctly

## 1.4.0 - 2022-08-29

* Added `traits` selector.
* Relative selectors (such as `above`, `below`, etc.) are now picking the closest element.
* Fix: continuous mode did not work for paths without a parent directory
* Fix: workaround for UiAutomator content descriptor crash
* Fix: `tapOn: {int}` did not work