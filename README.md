    # # # Distribution Statement A. Approved for public release. Distribution unlimited.
    # # #
    # # # Author:
    # # # Naval Research Laboratory, Marine Meteorology Division
    # # #
    # # # This program is free software: you can redistribute it and/or modify it under
    # # # the terms of the NRLMMD License included with this program. This program is
    # # # distributed WITHOUT ANY WARRANTY; without even the implied warranty of
    # # # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the included license
    # # # for more details. If you did not receive the license, for more information see:
    # # # https://github.com/U-S-NRL-Marine-Meteorology-Division/


CLAVR-x Test Datasets
==========================

This repository contains test datasets for use with the Geolocated Information Processing System.

Please see the 
[GeoIPS Documentation](https://github.com/NRLMMD-GEOIPS/geoips/blob/main/README.md)
for more information on the GeoIPS plugin architecture and base infrastructure.


Sample Dataset Sources
-----------------------

These CLAVR-x data files were produced at the Colorado State University Cooperative
Institute for Research in the Atmosphere.

* **License**: No constraints on data access or use.
* **Original CLAVR-x Development**: NOAA/NESDIS and the University of
  Wisconsin-Madison / CIMSS
* **Data Production and Algorithm Enhancements**: Colorado State University CIRA
* **CDR Program**: NOAA Climate Data Record Program for satellites


System Requirements
---------------------

* geoips >= 1.6.1
* Test data repos contained in $GEOIPS_TESTDATA_DIR for tests to pass.
   * test_data_clavrx >= 1.6.1
* GeoIPS Plugins:
   * geoips_clavrx >= 1.6.1


IF REQUIRED: Install base geoips package
------------------------------------------------------------
SKIP IF YOU HAVE ALREADY INSTALLED BASE GEOIPS ENVIRONMENT 

If GeoIPS Base is not yet installed, follow the
[installation instructions](https://github.com/NRLMMD-GEOIPS/geoips/blob/main/docs/installation.rst)
within the geoips source repo documentation.

Additionally, install all GeoIPS plugins and other packages specified in "System Requirements" above
(follow the installation instructions in their respective README files).

Obtain test repo
----------------
```bash
    # Assuming you followed the fully supported installation,
    # using $GEOIPS_TESTDATA_DIR and $GEOIPS_CONFIG_FILE:
    source $GEOIPS_CONFIG_FILE
    git clone https://github.com/NRLMMD-GEOIPS/test_data_clavrx $GEOIPS_TESTDATA_DIR/test_data_clavrx
```

Run sample test scripts
-----------------------
```bash

    # Assuming you followed the fully supported installation,
    # using $GEOIPS_TESTDATA_DIR, $GEOIPS_PACKAGES_DIR, and $GEOIPS_CONFIG_FILE:
    source $GEOIPS_CONFIG_FILE

    # GeoIPS-based test scripts should successfully return 0 if everything is set up properly.
    $GEOIPS_PACKAGES_DIR/geoips_clavrx/tests/test_all.sh
```
