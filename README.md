# Final Project

Zijian Ding, zding@ucsd.edu  
Yidi Zhu, yizhu@ucsd.edu  
Jishi Lyu, jlyu@ucsd.edu  
Changhao Shi, cshi@ucsd.edu

## Abstract Proposal

Our final project is to "make up" a classic movie scene Titanic - "I'm Flying" with style transfer and generative audio. It can be seen as a revisit of both Project 3 - Generative Audio and Project 4 - Generative Visual. The style transfer and generative audio will be conducted by GAN and DeepVoice3 model respectively. We hope to provide a new look of the movie scene: we will test different style type and audio model and select the best one. We will play this scene next Wednesday in the final project presentations.

## Project Report

Upload your project report (4 pages) as a pdf with your repository, following this template: [google docs](https://docs.google.com/document/d/133H59WZBmH6MlAgFSskFLMQITeIC5d9b2iuzsOfa4E8/edit?usp=sharing).

## Model/Data

Briefly describe the files that are included with your repository:
- trained models
In ChatterBot, we use the "chatterbot.corpus.english" set to train the robot. 
In DeepVoice, we download the pretrianed multi speaker synsethis model
("20171222_deepvoice3_vctk108_checkpoint_step000300000.pth").  
In ArbitraryStyleTransfer, we use the pretrained model and set the style weight to 2.0.

- training data (or link to training data)

## Code

Your code for generating your project:
- Jupyter notebooks: style_transfer_generative_code.ipynb, videoaudio_replacer.ipynb

## Results

Documentation of your results in an appropriate format, both links to files and a brief description of their contents:
- What you include here will very much depend on the format of your final project
  - image files (`.jpg`, `.png` or whatever else is appropriate)
  - 3d models
  - movie files (uploaded to youtube or vimeo due to github file size limits)
  - audio files
  - ... some other form

## Technical Notes

To build the ChatterBot: we need to clone the repository in:https://github.com/gunthercox/ChatterBot following the instructions to build your own chatterbot.(first pip install packages and build the setup file then download the 'en' of spacy)
When facing the warning of:  
/datasets/home/34/734/yizhu/.local/lib/python3.6/site-packages/chatterbot/corpus.py:38: YAMLLoadWarning: calling yaml.load() without Loader=... is deprecated, as the default Loader is unsafe. Please read https://msg.pyyaml.org/load for full details.
  return yaml.load(data_file)   
Please follow the instruction of the hint. 
To perform style transfer, please run style_transfer_generative_code.ipynb modified from https://github.com/elleryqueenhomels/arbitrary_style_transfer.
 
Any implementation details or notes we need to repeat your work. 
- Packages:
    cv2
- Does it run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Repositories
1.ChatterBot https://github.com/gunthercox/ChatterBot  
2.DeepVoicev3 https://github.com/r9y9/deepvoice3_pytorch
3.ArbitraryStyleTransfer https://github.com/elleryqueenhomels/arbitrary_style_transfer
