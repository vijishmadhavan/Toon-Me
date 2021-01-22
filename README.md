# [Toon-Me](https://github.com/vijishmadhavan/Toon-Me) &nbsp; [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Toon%20Portraits&url=https://github.com/vijishmadhavan/Toon-Me&via=Vijish68859437&hashtags=machinelearning,developers,100DaysOfCode,Deeplearning) &nbsp;


[![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](http://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)

**Mission**- A fun project to toon portrait images.

**Try your Twitter profile picture in the below colab link.** Read [Getting Started Yourself](#Getting-Started-Yourself) before trying (scroll down).

Best suited for **Twitter profile pictures**. Try **"Portrait"** photos below 550px.

Please try Model 1 before Model 2.

**Model 1:**

[<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/vijishmadhavan/Light-Up/blob/master/Toon_Me_(Alt_Model).ipynb)

**Model 2:** 

[<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/vijishmadhavan/Light-Up/blob/master/Toon_Me_(Try_it_on_Colab).ipynb)


## Highlights
- [Technical Details](#Technical-Details)
- [Getting Started Yourself](#Getting-Started-Yourself)
- [Try your Twitter profile picture on Colab](#Try-your-Twitter-profile-picture-on-Colab)



## Example Images

Hugh Jackman, actor

![Jackman](https://i.imgur.com/P3Z2ulm.jpg)

Robert Downey, Jr., American actor

![Robert](https://i.imgur.com/CmMlzER.jpg)

Jennifer Lawrence, American actress

![Jennifer Lawrence](https://i.imgur.com/6ZGNmdR.jpg)

Virat Kohli, Indian cricketer

![Virat](https://i.imgur.com/TcGTNgV.jpg)

Deepika Padukone, Indian actress

![Deepika](https://i.imgur.com/WOwjOsL.jpg)


## Toon-Me

Toon-Me is just a fun project, the main focus is to bring a cartoonized effect to profile pictures. Most of the profile pictures in twitter/Linkedin are portrait images as it helps with visibility, Toon-Me is well suited for images similar to profile pictures. Two models has been combined to bring the cartoonized effect, one is ArtLine https://github.com/vijishmadhavan/ArtLine and another one is Toon-Me.

**Technical details of ArtLine can be found on the below link.**

https://github.com/vijishmadhavan/ArtLine

## Technical Details

* **Progressive Resizing** (https://arxiv.org/abs/1710.10196),(https://arxiv.org/pdf/1707.02921.pdf). Progressive resizing takes this idea of gradually increasing the image size, In this project the image size were gradually increased and learning rates were adjusted. Thanks to fast.ai for intrdoucing me to Progressive resizing, this helps the model to generalise better as it sees many more different images.

* **Generator Loss** :  Perceptual Loss/Feature Loss based on VGG16. (https://arxiv.org/pdf/1603.08155.pdf).

* **No GAN** 

## Dataset

I have created a custom dataset having 300 images. 

## Getting Started Yourself

The easiest way to get started is to simply try out on Colab: [<img src="https://colab.research.google.com/assets/colab-badge.svg" align="center">](https://colab.research.google.com/github/vijishmadhavan/Light-Up/blob/master/Toon_Me_(Try_it_on_Colab).ipynb)

-Best suited for Twitter profile pictures. Try photos below 550px.

-Best suited for portrait photos in T-shirt/shirt (below 550px)

-Check the below given example image, poses similar to the below image are more suitable for better results.

![Imgur](https://i.imgur.com/OsqEEpR.jpg)

## Try your Twitter profile picture on Colab

Open colab run all the required cells, In case of doubt check this video.

https://www.youtube.com/watch?v=ULqlp6Btk2w&t=324s

Steps to Follow (Twitter/Linkedin):

1 Open your twitter profile page

2 Click on your profile picture, Let it expand.

3 Right click on the image

4 click on "copy image address".

5 Paste it on the url space provided, and run it.

![Imgur](https://i.imgur.com/rDjaWjx.jpg)

### Installation Details

This project is built around the wonderful Fast.AI library.

- **fastai==1.0.61** (and its dependencies).  Please dont install the higher versions
- **PyTorch 1.6.0** Please don't install the higher versions

### Limitations

- Output depends on Artline.
- Just Face cartoonization, nothing else.
- Some poses can be difficult for the model to asses.
- Good quality photos with proper lighting is needed for good results.
- Does not work well with random backgrounds, for better results need plain background portraits.


### Updates

[Get more updates on Twitter](https://twitter.com/Vijish68859437)

Mail me @ vijishmadhavan@gmail.com


