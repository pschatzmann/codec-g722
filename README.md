# arduino-libg722

[![Arduino Library](https://img.shields.io/badge/Arduino-Library-blue.svg)](https://www.arduino.cc/reference/en/libraries/)
[![IDF Component](https://img.shields.io/badge/IDF-Component-blue.svg)](https://github.com/pschatzmann/arduino-libg722)
[![CMake](https://img.shields.io/badge/CMake-Supported-blue.svg)](https://cmake.org/)

## Introduction

The G.722 module is a bit exact implementation of the ITU G.722 specification
for all three specified bit rates - 64000bps, 56000bps and 48000bps. It passes
the ITU tests.

To allow fast and flexible interworking with narrow band telephony, the
encoder and decoder support an option for the linear audio to be an 8k
samples/second stream. In this mode the codec is considerably faster, and
still fully compatible with wideband terminals using G.722.

## History

The code was originally written by Milton Anderson <milton@thumper.bellcore.com>
from BELLCORE, and has been modified by the Chengxiang Lu and Alex Hauptmann
from the Speech Group, School of Computer Science, Carnegie Mellon University,
to be fairly fast and efficient, while retaining high fidelity.

Steve Underwood <steveu@coppice.org> improved the code a lot later on and
contributed it into several popular open source projects.

Himanshu Soni <sonihimanshu@gmail.com> has adjusted some coefficients
to avoid over/under-flows in the decoder.

Phil Schatzmann <phil.schatzmann@gmail.com> has added cmake-glue and Arduino
support.

Librarized by Sippy Software, Inc.

## License

This code is mostly Public Domain. Library test code is under BSD 2-clause
license.

See LICENSE for copyright details and each individual file for specifics.
