# Annotation For Different Use Cases

CS.DataLabel supports various labeling methods for different use cases.

## Image Classiﬁcation Labelling Method

Draw a bounding box around an object and select a label for the object from the label list

![](../../.gitbook/assets/bbox.png)

## Text Recognition Labelling Method

Draw a bounding box around the text and insert the label into the blank label column

![](../../.gitbook/assets/bbox1.png)

## **Segmentation labeling method**

Draw a polygon around an object and assign a label for the object from the label list

![](../../.gitbook/assets/segmentation.png)

Create sub-labels for the current object if necessary by double-clicking the selected region

![](../../.gitbook/assets/sublabel.gif)

## **Export of Labels**

Annotation output has to be exported for the later process ****such as machine learning and deep learning. The types of saved output format depend on the supported formats to train the labeled data with. CS.DataLabel supports several output formats.

Click on the Save button to select the type of output format

![](../../.gitbook/assets/save%20%281%29.png)

## Bounding Box Annotation Output Format

![The output format of bounding box labeled data](../../.gitbook/assets/save-bbox.png)

{% hint style="warning" %}
Note: The option of saving label for current data point or the whole dataset is available for bounding box annotation
{% endhint %}

### Segmentation Annotation Output Format

![The output format of segmentation labeled data](../../.gitbook/assets/save-seg.png)

