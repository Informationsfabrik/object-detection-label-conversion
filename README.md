# object-detection-label-conversion

Resources for converting between labelling formats of image detection, with Python.

# Labelling formats

* CVAT XML
* COCO json
* [labelme](https://github.com/wkentaro/labelme)
* TFRecords
* VOC
* YOLO

# Convertion matrix

Links to convertion scripts (reads from left to right):

|               | CVAT XML | COCO json | Labelme | TFRecords | VOC | YOLO | 
| ------------- |:--------:|:-------:|:-------:|:---------:|:---:|:----:|
| **CVAT XML**  | ? | [CVAT](2) | ? | [CVAT](1) | [CVAT](3) | [CVAT](4) |
| **COCO json** | ? | ? | ? | ? | ? | ? |
| **labelme**   | ? | ? | ? | ? | ? | ? |
| **TFRecords** | ? | ? | ? | ? | ? | ? |
| **VOC**       | ? | ? | ? | ? | ? | ? |
| **YOLO**      | ? | ? | ? | ? | ? | ? |

[//]: <> (CVAT package)
  [1]: https://github.com/opencv/cvat/blob/master/utils/tfrecords/converter.md
  [2]: https://github.com/opencv/cvat/blob/master/utils/coco/converter.md
  [3]: https://github.com/opencv/cvat/blob/master/utils/voc/converter.md
  [4]: https://github.com/opencv/cvat/blob/master/utils/yolo/converter.md
