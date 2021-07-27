# Release Notes

## Classifai 1.2.0

_26 February 2021_

### What's New:

* **Shorcut Key Page** 

  Shortcut key page is now available, select the last button on the left panel to pop this window up 

![](https://user-images.githubusercontent.com/76682536/108791925-211fd300-75bb-11eb-84ad-b1d73d819ae5.png)

* **Malay language interface** 

  Malay language interface is now supported by Classifai

![](https://user-images.githubusercontent.com/76682536/108792232-bf139d80-75bb-11eb-9cb2-43e009c8f0df.png)

Toggle to different languages in the home interface. 

![Multilanguage supported](https://user-images.githubusercontent.com/33477318/108978768-eefa9800-76c4-11eb-82e1-66b52cbe20bb.gif)

### Enhancement:

* **Chinese language interface enhancement**

  There were some keywords failed to covered in the mandarin version earlier.  

  Now, the chinese language is fully translated with an enhancement of the keywords to best explain the functionalities.

  Before:

![](https://user-images.githubusercontent.com/76682536/108796627-1c135180-75c4-11eb-8c69-b61f73db7350.png)

After:

![](https://user-images.githubusercontent.com/76682536/108796383-9ee7dc80-75c3-11eb-98c6-2bdc4232b55e.png)

### Bug fixes:

* **Load Project without Data \(\#302\)**

  Previously progress update when loading project will occasionally complete without the data fully loaded. This is now fixed.

## **Classifai 1.1.1**

_29 January 2021_

### **Critical Fixes:**

* **Annotation output for bounding box projects changed to correspond to image name** \([\#277](https://github.com/CertifaiAI/classifai/issues/277)\) 

  The extension format of image, which previously concatenated into the annotation output of YOLO                 and Pascal VOC formats, is removed.



  Example 

  With image 1.jpg, the annotation output is 1.xml \(Prior to fix: 1\_jpg.xml\) 

  With image sample.jpg, the annotation output is sample.txt \(Prior to fix: sample\_jpg.txt\)



  Before:

![](https://user-images.githubusercontent.com/76682536/105820109-13931f80-5ff4-11eb-8cb3-7c37d9488583.gif)

         After:

![](https://user-images.githubusercontent.com/76682536/105820191-30c7ee00-5ff4-11eb-89e7-e0c43eef5b04.gif)

### **Other Fixes:**

* **JPEG aspect ratio fix** \([\#252](https://github.com/CertifaiAI/classifai/issues/252)\) 

  Previously, some jpeg files contain [EXIF orientation](https://www.impulseadventure.com/photo/exif-orientation.html) does not show the correct aspect ratio.  
  This is fixed in the current patch release.



  Before:

![](https://user-images.githubusercontent.com/76682536/105819925-d62e9200-5ff3-11eb-9599-4bc268342db1.png)

          After: 

![](https://user-images.githubusercontent.com/76682536/105819980-e3e41780-5ff3-11eb-899b-522dfd5d7d80.png)

* **JPEG timeout fix** \([\#280](https://github.com/CertifaiAI/classifai/issues/280)\) 

  Loading images with large size for bounding box or segmentation projects has previously resulted in timeout error.  
  This problem has been solved.



  Before: 

![](https://user-images.githubusercontent.com/76682536/105820048-0118e600-5ff4-11eb-9839-6af83111860e.gif)

        After: 

![](https://user-images.githubusercontent.com/76682536/105820078-08d88a80-5ff4-11eb-8296-bf0ea377b777.gif)

* **Enabling of detailed log messages if paths of images not found** \([\#283](https://github.com/CertifaiAI/classifai/issues/283)\) 

  When images previously imported could not be found in the system paths, the project will omit these images without causing any error. To give end users a better idea which images are missing, paths of images which cannot be found will be listed out in the log messages now.

![](https://user-images.githubusercontent.com/76682536/105820248-4806db80-5ff4-11eb-9cec-fe82b47c4cc9.png)

## **Classifai 1.1.0**

_11 January 2021_

### **What's New:**

* Deletion of project
* Deletion of data points by clicking on the images panel.

1. Open window for deleting data points by clicking on the image panel 

![](../.gitbook/assets/102965257-6f1b4a80-4528-11eb-9ae5-546223891ce4.png)

    2. Proceed with deleting images

![](https://user-images.githubusercontent.com/33477318/102965260-72163b00-4528-11eb-8ea1-7351608713bf.png)

### **Bug Fixes:**

* When import an empty folder in the first release \(version 1.0.0\) , Classifai was on the loading status forever. It is no longer the case with [bug fix](https://github.com/CertifaiAI/classifai/pull/226) from [\#223](https://github.com/CertifaiAI/classifai/issues/223)

## Classifai 1.0.0

14 November 2020

**What's New:** 

* Initial release of data annotation tool to public!

**Major features:**

* Images Annotation with
  * **Bounding Box** 
    * Classic Image Classification Problem:
      * Create labels on the right panel and assign label to object of interest
    * Text Recognition Use Cases \(OCR\):
      * Text creation straight into the label box
  * **Polygons** \(Segmentation\)
* Conversion of files format for easy annotation 
  * PDF /TIF -&gt; JPG/PNG 
* Distribution ready for easy installation on different operating systems:
  * Windows \(7, 8, 10\)
  * Mac
  * Ubuntu \(18 LTS, 20 LTS\)
  * Centos \(7, 8\)

![Image Classification Labelling Method: Assign labels created from Label List](../.gitbook/assets/woman.jpg)

![Text Recognition Labelling Method: Insert text into the blank label column](../.gitbook/assets/typescript.jpg)

