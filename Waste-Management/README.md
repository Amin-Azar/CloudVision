## This code has been modified from the repository mentioned below:

(https://github.com/maartensukel/urban-object-detection)


This repository combines elements from:
* https://github.com/zhaoyanglijoey/yolov3
* https://github.com/ultralytics/yolov3



## Installation

To install all required libaries:
```
pip install -r requirements.txt
```

### Pre trained weights

| Name | Classes          | Test data  |
| ------------- |:-------------:| -----:|
| 3 classes| cardboard, garbage_bags and containers| Yes |



### Run predictions

For example run the following the make a prediction on a file using CPU:

```
python detector_garb.py -i samples/input5_frame11.jpg -o output
```

Or to realtime detect on your webcam using GPU: (CUDA must be installed)
```
python detector_garb.py -i 0 --webcam --video -o ./webcam_output/ --cuda
```

### Docker

To run code in docker
```
docker-compose build
docker-compose up
```

