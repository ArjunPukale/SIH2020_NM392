# NM392_Neural-Architects
## PS: Depth Estimation of Valles Marineris using ISRO’s Mars Color Camera (MCC) images.
##
## Dataset Creation:
#### We were provided 7 images captured from ISRO's MCC camera of Valles Marineris.<br>To use Pix2Pix we need pair wise images of MCC image and corresponding Depth Map.<br>We used Nasa's MOLA Depth Map and superimposed that depth map on given MCC images.<br>We then used Image Augmentation to generate more pair wise images for our Dataset.<br>MOLA depth map link: https://astrogeology.usgs.gov/search/map/Mars/GlobalSurveyor/MOLA/Mars_MGS_MOLA_ClrShade_merge_global_463m
### We are Comparing different models for solving the above problem statement
### 1. Pix2Pix using Wessesterian Loss :
#### THE MODEL WAS TRAINED FOR 120 EPOCHS, USING WASSERSTEIN LOSS
![OUTPUT](https://github.com/ArjunPukale/SIH2020_NM392/blob/master/Images/Pix2pix%20Wloss.png)
### 2. Pix2Pix using Binary Cross Entropy :
#### THE MODEL WAS TRAINED FOR 120 EPOCHS, USING Binary Cross Entropy
![OUTPUT](https://github.com/ArjunPukale/SIH2020_NM392/blob/master/Images/Pix2pixBCE.PNG)
### 3. Sat2Map Pretrained Model
#### Pix2Pix using Pretrained weights used for SAT2MAP (satellite to map) task and training it on our dataset.
#### THE MODEL WAS TRAINED FOR 120 EPOCHS
![OUTPUT](https://github.com/ArjunPukale/SIH2020_NM392/blob/master/Images/Sat2map.png)


```
@inproceedings{CycleGAN2017,
  title={Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networkss},
  author={Zhu, Jun-Yan and Park, Taesung and Isola, Phillip and Efros, Alexei A},
  booktitle={Computer Vision (ICCV), 2017 IEEE International Conference on},
  year={2017}
}
```
