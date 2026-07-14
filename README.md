# QuPath_Pancreatic_Islet
This is a log for code, and how to use Qupath for creating workflows on classifying pancreatic islets. I will include errors that I encounter and my solutions to fix them. I will also include the resources that I used to become familiar with the software. 
Resources that I've used so far: https://qupath.readthedocs.io/en/stable/ 
Good youtube course: https://www.youtube.com/watch?v=MBrAVUsUdio&list=PLSCpSsEmyRpANBGQXB_oGslW9NIJz4A12
Jargon:
JavaFX interface: instead of using terminal, a JavaFX interface makes it so you can drag and click to use the software.
Compatible with other open-source tools:
  Imagej
    - You can send images and ROIs between QuPath and imajeJ this allows for to use an ImageJ specific tool or vice-versa
    - Are able to use plug-ins built in for imajeJ on QuPath depending if you find code already built for imageJ
    - Can open TIFF file types (these contain metadata): both can open in imajeJ and QuPath
  OpenCV
    - Library with pre-built tools 
      - edge detection
      - filtering 
      - blurring 
      - contour finding 
      - morphological operations: expanding/shrinking shapes, filling holes etc
      - QuPath already uses some of these tools in its software
  Java Topology Suite
    - Another library
      - Good for geometry
      - For islet quantification:
        - This software handles area, perimeter, and roundness calculations
        - Used to see if theres another shape within another i.e. glucagon overlapping with insulin
        - Merges, splits, or simplifies shapes
        - Handles overlap/intersection
  OMERO
    - server-based system for storing nd organizing large microscopy images 
    - Labs generating lots of data should be use OMERO for storing large datasets 
    -  link for OMERO 
    
