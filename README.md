# Oasis 500M

![](./media/arch.png)

![](./media/thumb.png)

Oasis is an interactive world model developed by [Decart](https://www.decart.ai/) and [Etched](https://www.etched.com/). Based on diffusion transformers, Oasis takes in user keyboard input and generates gameplay in an autoregressive manner.

This repo forks someone else's repo which they forked from the original. This one contains patches and can run properly. I will include a ready to use offline model soon.

If you want to use the original live demo, be sure to check out the [live demo](https://oasis.us.decart.ai/) there.

## Setup
```
git clone https://github.com/dgrtygry2/open-oasis.git
cd open-oasis
# Install pytorch
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
# Install other dependencies
pip install einops diffusers timm av
```
To download a premade version of this program with the models, Go to the releases.
```

## Basic Usage
Only use this if you are training any data. run "game.py" if you want to play the game offline.
```
python generate.py
```
The resulting video will be saved to `video.mp4`. Here's are some examples of a generation from this 500M model!

![](media/sample_0.gif)
![](media/sample_1.gif)

> Hint: try swapping out the `.mp4` input file in the script to try different environments!
