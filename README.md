# MobileGFXSetup

Welcome to Mobile GFX Setup!

## Introduction

Mobile GFX Setup generates all of the mobile icons, spotlights, settings and launchers for Delphi Android and iOS applications.

## How to use Mobile GFX Setup

 1. Set up your images on the Graphics tab
* For each image ratio, enter or browse to an image file
* Select the part of the image to be used for the format
* Move the image selection around by Ctrl dragging the red rectangle

 2. Set up the output options from the Setup tab
* Enter a base filename for the generated images. The tool will append the width and height of an image to this filename (e.g., `c:\junk.png` becomes `c:\junk114x114.png`)
* Select which devices you want to generate images for
* Finally, check the **Generate .optset file(s)** checkbox if you want the .optset file generated which you can then later import into Delphi

 3. Generate your images from the Generate tab
* When you go to the Generate tab, the tool will verify you have entered everything correctly
* If validation has passed, click the **Generate** button to generate the images and, optionally, the .optset files (which will be called basename.android.optset and basename.ios.optset)

 4. Finished!

If you generated the .optset file, do the following steps:

* Load your Delphi project
* Select *Project > Options* to show the project options
* Click **Application** on the left to show application options
* Change the Target configuration
* Click the **Apply...** button
* Browse to the .optset file
* Modify the configuration and click OK!

## History

Tom Grubb [created this project on February 3, 2014](http://blogs.riversoftavg.com/index.php/2014/02/03/creating-icons-and-launchers-for-delphi-mobile-applications/).

Graham Murt [modified this project on February 5, 2015](http://riversoftavg.com/blogs/index.php/2014/02/03/creating-icons-and-launchers-for-delphi-mobile-applications/#comments):
* Added extra image sizes (87x87, 180x180, 750x1334, 1242x2280, 2208x1242)
* Added some code to load/save the filenames to an ini file so that the previous selection is remembered when run.

Tom Grubb [modified this project on February 7, 2015](http://riversoftavg.com/blogs/index.php/2015/02/07/creating-icons-and-launchers-for-delphi-mobile-applications-redux/):
* Extended Graham's update a little bit for the Android splash images and persisting the rectangles as well.