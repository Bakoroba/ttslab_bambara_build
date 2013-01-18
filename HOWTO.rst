=========================================
How to build a slot-and-filler TTS system
=========================================

1. Introduction
===============

This document describes the process of building a simple
slot-and-filler TTS system from the current resource using TTSLab and
TTSLabdev tools. This is done by automatically processing the audio
resources to create an audio database of words that are then used to
synthesise sentences with varying content.


2. Software setup
=================

2.1. External dependencies
--------------------------

In order to build this system a GNU/Linux system with various speech
processing utilities is required. Before continuing please ensure that
the following are installed.

The following software can easily be installed from your Linux
distribution's software repository and should be on your system path:

- Python 2.7 or higher
- Numpy
- Scipy
- SoX
- normalize-audio (http://normalize.nongnu.org/)
- Praat (http://www.fon.hum.uva.nl/praat/)

In addition, the following software should be downloaded from the
given locations and built appropriately. There is no need to install
these to your system, further information will be provided where paths
to these packages can be configured:

- HTK 3.4.1 (http://htk.eng.cam.ac.uk/)
- Edinburgh Speech Tools 2.1 (http://www.cstr.ed.ac.uk/downloads/festival/2.1/speech_tools-2.1-release.tar.gz)


2.2. Setting up TTSLab and TTSLabdev
------------------------------------

