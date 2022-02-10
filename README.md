# Object_Detection_SSD_TF2
A TensorFlow 2.4.1 implementation of Single Shot MultiBox Detector (SSD).
This project is refer [it](https://github.com/calmisential/TensorFlow2.0_SSD). 

## Requirements
- Python >=3.8
- TensorFlow >=2.4.1

### Implement detail (author)
- OS      :Windows 10 with ANACONDA
- GPU     :NVIDIA GeForce RTX 3060
- CPU     :Intel(R) Core(TM) i5-9400F @ 2.90GHz
- Dataset :SnacksMIT   

## Usage
### TrainVal
1. Prepared your dataset. For instance, PASCAL VOC dataset.
2. Put the dataset in the "dataset" folder. Then, make sure the directory is like this:
```
|---dataset
     |---VOCdevkit
          |---VOC2012
                |---Annotations
                |---ImageSets
                |---JPEGImages
                |---SegmentationClass
                |---SegmentationObject
```
3. Check all the value of the parameters in `configuration.py`.
4. Generate the file for training. Run `write_voc2txt.py` to generate voc.txt.
5. Start training. Run `train.py` to start training.

### Test
1. Modified the value of the parameters in `configuration.py`. (p.s. test_picture_dir)
2. Run `test.py` to test on single picture.

## Reference
- SSD:Single Shot MultiBox Detector [#LINK](https://arxiv.org/abs/1512.02325)
- Github/calmisential/TensorFlow2.0_SSD [#LINK](https://github.com/calmisential/TensorFlow2.0_SSD)
