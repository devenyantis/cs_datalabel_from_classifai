# Project Import/Export

A project can be imported into CS.DataLabel using a conﬁguration ﬁle in **JSON format**. The conﬁguration ﬁle contains the metadata of a project to reproduce it in a different system.

{% hint style="danger" %}
**The conﬁguration ﬁle of a project comes from the export feature of CS.DataLabel** **tool.**
{% endhint %}

### Beneﬁts of the Import/Export Feature:

1. Visual cross-validation on image labeling quality
2. Reimport project to adjust, remove, or add labels to reannotate the undesired labeled images
3. Reimport project to output user-preferred label formats such as YOLO and Pascal VOC
4. Customizable image annotation for different projects
5. Flexible collaboration between labeler and engineer
6. All images annotation data will be updated and saved to the CS.DataLabel database, this prevents the user from losing valuable labeled images data and time

### Methods:

### How to Export Project Conﬁguration File:

The project can be exported in two options.

1. **Conﬁg ﬁle:** Save a JSON format ﬁle into the project folder.
2. **Zip File \(with data\):** Save all the images together with the project JSON ﬁle into one zip ﬁle.

![](../../.gitbook/assets/export-project.gif)

### How to Import Project Conﬁguration File:

Import by selecting the conﬁguration ﬁle in JSON format.

![Select Import project](../../.gitbook/assets/import.png)

![](../../.gitbook/assets/import-project.png)

![Choose the project configuration file \(.json\) in the image folder](../../.gitbook/assets/config-file.png)

![Project imported](../../.gitbook/assets/imported.png)

