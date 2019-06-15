# Final Project

Zijian Ding, zding@ucsd.edu  
Yidi Zhu, yizhu@ucsd.edu  
Jishi Lyu, jlyu@ucsd.edu  
Changhao Shi, cshi@ucsd.edu

## Abstract Proposal

Our final project is to "make up" a classic movie scene Titanic - "I'm Flying" with style transfer and generative audio. It can be seen as a revisit of both Project 3 - Generative Audio and Project 4 - Generative Visual. The style transfer and generative audio will be conducted by GAN and DeepVoice3 model respectively. We hope to provide a new look of the movie scene: we will test different style type and audio model and select the best one. We will play this scene next Wednesday in the final project presentations.

## Project Report



## Model/Data

Briefly describe the files that are included with your repository:

- In ChatterBot, we use the "chatterbot.corpus.english" set to train the robot. 

- In DeepVoice, we download the pretrianed multi speaker synsethis model.
("20171222_deepvoice3_vctk108_checkpoint_step000300000.pth").

- In ArbitraryStyleTransfer, we use the pretrained model and set the style weight to 2.0.

## Code

Your code for generating your project:
- Style transfer: style_transfer_generative_code.ipynb, 
- ChatterBot and audio generation: videoaudio_replacer.ipynb

## Results
![question](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/Doyoutrustme.png)
![generated answer](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/Sortof.png)
The final artwork is uploaded to YouTube: 
https://www.youtube.com/watch?v=bkWVaSbXI4w

## Technical Notes

- ChatterBot & Audio Generation

To build the ChatterBot, clone the repository in:https://github.com/gunthercox/ChatterBot. Follow the instructions to build your own chatterbot.(first pip install packages and build the setup file then download the 'en' of spacy)
When facing the warning: YAMLLoadWarning: calling yaml.load() without Loader=... is deprecated, as the default Loader is unsafe. Please read https://msg.pyyaml.org/load for full details.
  return yaml.load(data_file)   
Please follow the instruction of the hint.

- Style Transfer

To perform style transfer, please run style_transfer_generative_code.ipynb modified from https://github.com/elleryqueenhomels/arbitrary_style_transfer.
 
Required package: cv2

## Reference

References to repositories we used:

1.ChatterBot https://github.com/gunthercox/ChatterBot  

2.DeepVoicev3 https://github.com/r9y9/deepvoice3_pytorch

3.ArbitraryStyleTransfer https://github.com/elleryqueenhomels/arbitrary_style_transfer
