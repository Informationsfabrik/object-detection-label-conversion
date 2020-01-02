# object-detection-label-conversion

Resources for converting between labelling formats of image detection, with Python.

# Labelling formats

Dataset formats:
* COCO json
* Pascal VOC

Annotation-tool formats:
* CVAT XML
* [labelme](https://github.com/wkentaro/labelme)

Model-specific formats:
* TFRecords
* YOLO

# Script-based conversion

Links to convertion scripts (reads from left to right):

|  &#8625;       | CVAT XML | COCO json | labelme | TFRecords | Pascal VOC | YOLO | 
| -------------- |:--------:|:-------:|:-------:|:---------:|:---:|:----:|
| **CVAT XML**   | - | [CVAT](2) | ? | [CVAT](1) | [CVAT](3) | [CVAT](4) |
| **COCO json**  | ? | - | ? | [Tensorflow](11) | [carolinepacheco](14) | [convert2Yolo](7) |
| **labelme**    | ? | [annotation_utils](5) | - | ? | [labelme](6) | [LabelmeToYolo](8) |
| **TFRecords**  | ? | ? | ? | - | ? | ? |
| **Pascal VOC** | ? | [soumenpramanik](13) | ? | [Tensorflow](12) | - | [convert2Yolo](7), [goodhamgupta](10) |
| **YOLO**       | ? | ? | ? | ? | [goodhamgupta](9) | - |

[//]: # (CVAT package)
  [1]: https://github.com/opencv/cvat/blob/master/utils/tfrecords/converter.md
  [2]: https://github.com/opencv/cvat/blob/master/utils/coco/converter.md
  [3]: https://github.com/opencv/cvat/blob/master/utils/voc/converter.md
  [4]: https://github.com/opencv/cvat/blob/master/utils/yolo/converter.md
[//]: # (annotation_utils)
  [5]: https://github.com/cm107/annotation_utils/blob/master/build/lib/annotation_utils/converter/labelme_coco_converter.py
[//]: # (labelme)
  [6]: https://github.com/wkentaro/labelme/blob/master/examples/bbox_detection
[//]: # (LabelmeToYolo)
  [8]: https://github.com/heleizj/LabelmeToYolo
[//]: # (convert2Yolo)
  [7]: https://github.com/SsaRu/convert2Yolo
[//]: # (goodhamgupta)
  [//]: # (YOLO to VOC:)
  [9]: https://gist.github.com/goodhamgupta/7ca514458d24af980669b8b1c8bcdafd
  [//]: # (VOC to YOLO:)
  [10]: https://gist.github.com/goodhamgupta/eb5b4cdd22fa95341502e1187ec71849
[//]: # (TF Object Detection API)
  [11]: https://github.com/tensorflow/models/blob/master/research/object_detection/dataset_tools/create_coco_tf_record.py
  [12]: https://github.com/tensorflow/models/blob/master/research/object_detection/dataset_tools/create_pascal_tf_record.py
[//]: # (soumenpramanik)
  [13]: https://github.com/soumenpramanik/Convert-Pascal-VOC-to-COCO/blob/master/convertVOC2COCO.py
[//]: # (carolinepacheco)
  [14]: https://github.com/carolinepacheco/Convert-COCO-to-PascalVOC

# Tool-based conversion

The labelling tool [CVAT appears to have](https://github.com/opencv/cvat) good support for importing and exporting (thus converting) various annotation formats.
