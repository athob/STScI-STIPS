#############
Release Notes
#############

Version History and Change Log
-------------------------------

Version 1.0.8
=============
*2020 Date TBD*

- Future changes here

Version 1.0.7
=============
*2019 January 8*

**STIPS Improvements**

- Cookie cutter template used to create better package infrastructure. [:pr:`40`, :user:`robelgeda`]
- Docker file added for ease of install. [:pr:`48`, :user:`robelgeda`]
- environment.yml added for easy conda env build. [:pr:`42`, :user:`robelgeda`]
- Read the Docs documentation established. [:pr:`55`, :user:`robelgeda`]
- F062 filter added to WFIRST WFI. [:pr:`51`, :user:`york-stsci`]
- Update STIPS to use WbbPSF 0.9.0. [:pr:`51`, :user:`york-stsci`]
- Travis CI initiated for unit and regression testing. [:pr:`40`, :user:`robelgeda`]
- Python version set to 3.7 [:pr:`40`, :user:`robelgeda`]
- Licenses updated [:pr:`40`, :user:`robelgeda`]

**General bug fixes and small changes**

- Updated astro_image.py to use a PC matrix rather than a CD matrix for the image WCS, which hopefully will result in astropy actually giving you a correctly formatted FITS WCS. [:pr:`46`, :user:`york-stsci`]
- Adding WCS information to PSF files. PSF files will now have the following:
    - RA equal to the observation RA at which they were produced
    - DEC equal to the observation DEC at which they were produced
    - PA equal to the observation PA at which they were produced
    - CDELT keywords equal to the PIXELSCL keyword, but adjusted to degrees rather than arcsec.
    - [:pr:`47`, :user:`york-stsci`]
