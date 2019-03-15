# How to make historical data useful and usable in GIS for spatial analyses

**Fiducial marks:** reference marks also called Réseau crosses

## Further Steps

### Human assisted corrections DONE!
Find and correct errors
 - Images flipped or/and rotated
- ...

### OpenCV - Open Source Computer Vision Library

[OpenCV](https://opencv.org/)  
[opencv4nodejs](https://www.npmjs.com/package/opencv4nodejs)

Use Computer Vission techniques to identify features:
- **Fiducial marks:** reference marks also called Réseau crosses
- Cost lines
- ...

### GDAL - Geospatial Data Abstraction Library

[GDAL](https://www.gdal.org/)  

    sudo apt-get install gdal-bin

Tiff --> GeoTiff with (gdal_translate)

    gdal_translate -of GTiff -a_srs EPSG:4326 -gcp [pixel line easting northing] -gcp [pixel line easting northing] -gcp [pixel line easting northing] -gcp [pixel line easting northing] sourcefile outpulfile

ex.

    gdal_translate
      -of GTiff
      -a_srs EPSG:4326
      -gcp 0 0 -59.58761675889423 -51.61091493867437
      -gcp 11671 0 -59.504807792918086 -51.609144921878766
      -gcp 11671 12065 -59.50197069288032 -51.66052445469222
      -gcp 0 12065 -59.58482493888437 -51.66232361748121
    F_I_15_0024.jpg
    F_I_15_0024.tif

### ODM - Drone Mapping Software

[OpenDroneMap](https://www.opendronemap.org/)  
[Node-ODM](https://github.com/OpenDroneMap/OpenDroneMap)

Generate a mosaic

## Previous uses of these aerial photographs

###  Picking Up Penguins From Space

[Picking Up Penguins From Space](https://www.pixalytics.com/picking-penguins-space/)  

Historical aerial photographs: Images taken by Falkland Islands Dependencies Aerial Survey Expedition (FIDASE) on the 31st January 1957 were digitally scanned and geo-referenced to the WorldView-2 data. They were then divided into polygons and analysed using manual classification processing using the open source QGIS software.

## Original Source

### Falkland Islands and Dependencies Aerial Survey Expedition

This comprises approximately 12,800 frames, taken on 26,700 kilometres of ground track. The photography was acquired between February 1956 and December 1957. The images are vertical, monochrome photographs in the standard 9" x 9" format; some small format (5" x 5") oblique photographs are also available for a restricted geographical coverage. The original negatives are held by BAS. The photography provides systematic coverage of the South Shetland Islands and the west side of the Antarctic Peninsula as far south as the northern extremity of Marguerite Bay.

Flight-line index maps are available for most of the coverage. For details of holdings of a particular area, please contact:

    Mrs Janet W. Thomson
    Head of the Mapping and Geographic Information Centre
    British Antarctic Survey
    High Cross Madingley Road
    CAMBRIDGE CB3 OET
    UNITED KINGDOM
    telephone: +44 (0)1223 221424
    e-mail: jwth@bas.ac.uk

Contact prints of the FIDASE photography can be ordered through Mrs Thomson.
Permission will be required from all of the authorities named above to reproduce any supplied photograph.

## References

[Basic Concepts of Aerial Photography](https://www.nrcan.gc.ca/earth-sciences/geomatics/satellite-imagery-air-photos/air-photos/about-aerial-photography/9687)  
[Aerial Survey Expedition 1955-57](https://www.asprs.org/wp-content/uploads/pers/1958journal/jun/1958_jun_415-427.pdf)  
[Multi-modal survey of Adélie penguin mega-colonies reveals the Danger Islands as a seabird hotspot](https://www.nature.com/articles/s41598-018-22313-w)
