# Change Log AS5600
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).


## [0.3.4] - 2022-12-22
- fix #26 edges problem of the experimental cumulative position (CP).
- decoupled CP from **rawAngle()**
  - now one needs to call **getCumulativePosition()** to update the CP.
- updated the readme.md section about CP.


## [0.3.3] - 2022-12-19
- add experimental continuous position.
  - add **getCumulativePosition()**
  - add **resetPosition()**
  - add **getRevolutions()**
- move code from .h to .cpp
- add AS5600_MODE_RPM to **getAngularSpeed()**
- add AS5600_RAW_TO_RPM
- add example for AS5600_MODE_RPM.
- add AS5600_DEFAULT_ADDRESS
- add AS5600L_DEFAULT_ADDRESS
- update readme.md

## [0.3.2] - 2022-10-16
- add CHANGELOG.md
- update readme.md
- update build-CI to support RP2040

## [0.3.1] - 2022-08-11
- add support for AS5600L (I2C address)
- add magnetTooStrong() + magnetTooWeak();
- add / update examples
- update documentation

## [0.3.0] - 2022-07-07
- fix #18 invalid mask setConfigure().

----

## [0.2.1] - not released
- add bool return to set() functions.
- update Readme (analog / PWM out)

## [0.2.0] - 2022-06-28
- add software based direction control.
- add examples
- define constants for configuration functions.
- fix conversion constants (4096 based)
- add get- setOffset(degrees)   functions. (no radians yet)

----

## [0.1.4] - 2022-06-27
- fix #7 use readReg2() to improve I2C performance.
- define constants for configuration functions.
- add examples - especially OUT pin related.
- fix default parameter of the begin function.

## [0.1.3] - 2022-06-26
- add AS5600_RAW_TO_RADIANS.
- add getAngularSpeed() mode parameter.
- fix #8 bug in configure.

## [0.1.2] - 2022-06-02
- add getAngularSpeed().

## [0.1.1] - 2022-05-31
- add readReg2() to speed up reading 2 byte values.
- fix clock wise and counter clock wise.
- fix shift-direction @ getZPosition, getMPosition,
  getMaxAngle and getConfigure.

## [0.1.0] - 2022-05-28
- initial version

