# Toon-Me

[![forthebadge](https://forthebadge.com/images/badges/open-source.svg)](http://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)

**Mission**- A fun project to toon profile pictures.

**Try your Twitter/Linkedin profile picture in the below colab link.**

## Example Images

Robert Downey, Jr., American actor

![Robert](https://i.imgur.com/CmMlzER.jpg)

Virat Kohli, Indian cricketer

![Virat](https://i.imgur.com/TcGTNgV.jpg)

Tom Cruise, American actor

![Tom](https://i.imgur.com/2VFw4h3.jpg)

Aamir Khan, Indian actor

![Amir](https://i.imgur.com/G7z6k2M.jpg)

Deepika Padukone, Indian actress

![Deepika](https://i.imgur.com/WOwjOsL.jpg)


## Toon-Me

Toon-Me is just a fun project, the main focus is to bring a cartoonized effect to profile pictures. Most of the profile pictures in twitter/linkedin are portrait images as it helps in visibility, Toon-Me is well suited for images similar to profile pictures. Two models has been combined to bring the cartoonized effect, one is ArtLine https://github.com/vijishmadhavan/ArtLine and another one is Toon-Me.

**Technical details of ArtLine can be found on the below link.**

https://github.com/vijishmadhavan/ArtLine

## Technical Details

* **Progressive Resizing** (https://arxiv.org/abs/1710.10196),(https://arxiv.org/pdf/1707.02921.pdf). Progressive resizing takes this idea of gradually increasing the image size, In this project the image size were gradually increased and learning rates were adjusted. Thanks to fast.ai for intrdoucing me to Progressive resizing, this helps the model to generalise better as it sees many more different images.

* **Generator Loss** :  Perceptual Loss/Feature Loss based on VGG16. (https://arxiv.org/pdf/1603.08155.pdf).

* **No GAN** 


## Dataset

I have created a custom dataset having 300 images. 

### Limitations

- Output depends on Artline.
- Just Face cartoonization, nothing else.
- Some poses can be difficult for the model to asses.
- Good quality photos with proper lighting is needed for good results.
