# Some ideas to improve modelling

- Due to the large difference in image size, rescaling may not be the best preprocessing.
  It might be useful to use black or white as padding (and teaching the NN to ignore it)
  Rescaling might produce artifacts, reduce a characteristic
  or distract the NN by enlarging something irrelevant like water.



# NN Arch

- Learning similarity:
    - Siamese Networks: https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf
    - Generative Adversarial Network
    - Triplet network
      - https://arxiv.org/abs/1412.6622
      - https://arxiv.org/abs/1804.07275v1
      - Quadruplet Loss: https://arxiv.org/abs/1704.01719
      - Histogram Loss: https://arxiv.org/abs/1611.00822
- Matching network: https://arxiv.org/abs/1606.04080
- Re-Identification networks
  - https://github.com/KaiyangZhou/deep-person-reid and https://github.com/KaiyangZhou/deep-person-reid/blob/master/AWESOME_REID.md
- Meta learning: https://openreview.net/pdf?id=rJY0-Kcll
- Neural Turing Machine
      - https://arxiv.org/pdf/1410.5401
      - One shot learning: https://arxiv.org/abs/1605.06065
- Unsupervised pretraining: http://www.jmlr.org/papers/volume11/erhan10a/erhan10a.pdf
  - Pretraining with an autoencoder
  - Not gradient based
    - Restricted Boltzmann machine & Deep Belief Network
    - Conditional Random Field
- Multi stage with a segmentation/Region Proposal network and then a predictor on the crops

- Training from Scratch: https://arxiv.org/pdf/1811.08883.pdf

# Leaks

As always, your usual image leak ...


```
fffde072b.jpg        File name       : fffde072b.jpg
fffde072b.jpg        File size       : 252346 Bytes
fffde072b.jpg        MIME type       : image/jpeg
fffde072b.jpg        Image size      : 1000 x 652
fffde072b.jpg        Camera make     : Canon
fffde072b.jpg        Camera model    : Canon EOS 7D Mark II
fffde072b.jpg        Image timestamp : 2016:08:14 15:43:25
fffde072b.jpg        Image number    : 
fffde072b.jpg        Exposure time   : 1/2000 s
fffde072b.jpg        Aperture        : F8
fffde072b.jpg        Exposure bias   : 0 EV
fffde072b.jpg        Flash           : No, compulsory
fffde072b.jpg        Flash bias      : 
fffde072b.jpg        Focal length    : 400.0 mm
fffde072b.jpg        Subject distance: Infinity
fffde072b.jpg        ISO speed       : 400
fffde072b.jpg        Exposure mode   : Shutter priority
fffde072b.jpg        Metering mode   : Multi-segment
fffde072b.jpg        Macro mode      : 
fffde072b.jpg        Image quality   : 
fffde072b.jpg        Exif Resolution : 5472 x 3648
fffde072b.jpg        White balance   : Auto
fffde072b.jpg        Thumbnail       : image/jpeg, 5680 Bytes
fffde072b.jpg        Copyright       : © Jodi Frediani
fffde072b.jpg        Exif comment    : 

e6085534a.jpg        File name       : e6085534a.jpg
e6085534a.jpg        File size       : 150642 Bytes
e6085534a.jpg        MIME type       : image/jpeg
e6085534a.jpg        Image size      : 761 x 435
e6085534a.jpg        Camera make     : Canon
e6085534a.jpg        Camera model    : Canon EOS 350D DIGITAL
e6085534a.jpg        Image timestamp : 2006:10:08 13:44:19
e6085534a.jpg        Image number    : 
e6085534a.jpg        Exposure time   : 1/500 s
e6085534a.jpg        Aperture        : F10
e6085534a.jpg        Exposure bias   : 0 EV
e6085534a.jpg        Flash           : No, compulsory
e6085534a.jpg        Flash bias      : 
e6085534a.jpg        Focal length    : 300.0 mm
e6085534a.jpg        Subject distance: 
e6085534a.jpg        ISO speed       : 200
e6085534a.jpg        Exposure mode   : Auto
e6085534a.jpg        Metering mode   : Multi-segment
e6085534a.jpg        Macro mode      : 
e6085534a.jpg        Image quality   : 
e6085534a.jpg        Exif Resolution : 864 x 576
e6085534a.jpg        White balance   : Auto
e6085534a.jpg        Thumbnail       : image/jpeg, 5978 Bytes
e6085534a.jpg        Copyright       : 
e6085534a.jpg        Exif comment    : 

cc6c1a235.jpg        File name       : cc6c1a235.jpg
cc6c1a235.jpg        File size       : 256573 Bytes
cc6c1a235.jpg        MIME type       : image/jpeg
cc6c1a235.jpg        Image size      : 1050 x 700
cc6c1a235.jpg: No Exif data found in the file
b22ded8a8.jpg        File name       : b22ded8a8.jpg
b22ded8a8.jpg        File size       : 184932 Bytes
b22ded8a8.jpg        MIME type       : image/jpeg
b22ded8a8.jpg        Image size      : 1050 x 467
b22ded8a8.jpg: No Exif data found in the file
```