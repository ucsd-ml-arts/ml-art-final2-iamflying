# Final Project: “A Picture of Him” - Video Style Transfer and Chatbot Audio Generation

Zijian Ding, zding@ucsd.edu  
Yidi Zhu, yizhu@ucsd.edu  
Jishi Lyu, jlyu@ucsd.edu  
Changhao Shi, cshi@ucsd.edu

## Abstract

“I don't even have a picture of him. He exists now only in my memory." The moving lines of Rose in Titanic have touched thousands of people deeply. In this project, we hope to eliminate the regret of Rose by applying style transfer to generate the scene of Jack and Rose “I’m flying”. To make the scene more interesting, we also use chatbot audio generation to produce new lines of the scene.

It can also be seen as a revisit of both Project 3 - Generative Audio and Project 4 - Generative Visual. The style transfer and generative audio will be conducted by GAN and DeepVoice3 & ChatterBot model respectively.

## Project Report
It is uploaded to this repo.

## Model/Data

Briefly describe the files that are included with your repository:

- In ChatterBot, we use the "chatterbot.corpus.english" set to train the robot. 

- In DeepVoice, we download the pretrianed multi speaker synsethis model.
("20171222_deepvoice3_vctk108_checkpoint_step000300000.pth").

- In ArbitraryStyleTransfer, we use the pretrained model and set the style weight to 2.0.

## Code

Codes for generating your project:
- Style transfer: style_transfer_generative_code.ipynb, 
- ChatterBot and audio generation: videoaudio_replacer.ipynb

## Results
We have tried several style image and selected the best effect. Also, for the audio generation we tried different inputs. More details are discussed in our report.

The final artwork is uploaded to YouTube: 
https://www.youtube.com/watch?v=bkWVaSbXI4w

Here is an example of the text generated by the chatter bot. 
The screenshot for original question is:

![question](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/Doyoutrustme.png)

The original answer is “I trust you”; while the generated one is “sort of” as shown in the screenshot:

![generated answer](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/Sortof.png)

More selected screenshots are attached below:

![generated answer](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/example1.png)

![generated answer](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/example2.png)

![generated answer](https://github.com/ucsd-ml-arts/ml-art-final2-iamflying/blob/master/some_example/example3.png)

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

1. ChatterBot https://github.com/gunthercox/ChatterBot  

2. DeepVoicev3 https://github.com/r9y9/deepvoice3_pytorch

3. ArbitraryStyleTransfer https://github.com/elleryqueenhomels/arbitrary_style_transfer
