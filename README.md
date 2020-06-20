# road sign tagging

Tagging the images which has the road signs like

![example of road signs](https://www.guide2dubai.com/Portals/0/Images/Living/Transportation/dubai-road-signs.jpg)


### Installation


downlaod the pre-trained road sign detection model from the url 



to install the cheque detector model, you need Python 3.7.7 

```bash
git clone https://github.com/gaoyuanliang/road_sign_tagging.git

cd road_sign_tagging

pip3 install -r requirements.txt

wget https://github.com/fchollet/deep-learning-models/releases/download/v0.4/xception_weights_tf_dim_ordering_tf_kernels_notop.h5
```

download the pretrain model of cheque detection from the following url

```
https://drive.google.com/file/d/1lGkgRc1VU1tVJPiMUSVyCV2Elm1Gy8_-/view?usp=sharing
```

### Using

down load an image of road sign 

```base
wget https://c8.alamy.com/comp/FPMFN8/road-signs-dubai-uae-FPMFN8.jpg
```

import the model in python3

```python
from road_sign_tagging import road_sign_tagging
```

run the tagging program

```python
road_sign_tagging('road-signs-dubai-uae-FPMFN8.jpg')
```

you will see the following output:

```python
{'tag': 'road_sign', 'score': 0.9429549}
```
