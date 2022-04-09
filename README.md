# Spectrogram Generator

This repository holds all code produced by the VIP dolphin acoustics group that are relevant to the generation of datasets for machine learning. As of April 9th 2022, the group's main focus is to use spectrograms of waveform clips to train their models. But in the future this repository can be expanded to contain preprocessing methods on waveform data files. 

We used jupyter notebooks as our working environments for the code. If you type githubtocolab in place of github in the url of the jupyter notebook you are currently reading, you can automatically jump to google colab.

## Set up

The easiest way to set up and run the jupyter notebook files in this folder is by creating a virtual environment for this project. This way you can avoid the so-called "dependency-hell". For a tutorial head to this [link](https://github.com/dolphin-acoustics-vip/Workflow_Tutorials#creating-a-virtual-environment-using-virtualenv-python-specific).
But you can obviously choose your own preferred way of getting everything set up, just know that it will be more work.

The Python version used in this project is Python 3.9.10

Each file is self contained, and they don't require any extra modules to import or download apart from those pippable in the requirements.txt file.

The code here is fully os-independent, so you don't have to worry whether you are running on a windows os or IOS or linux, they will all work. But do make sure you set up a virtual environment correctly before continuing.

## What does each file do?

Quick overview:

[dataset_generator.ipynb](https://github.com/dolphin-acoustics-vip/Spectrogram-Generator/blob/main/dataset_generator.ipynb): This jupyter notebook is for everything related to generating spectrograms:
- finding clips in the given input path
- generating and saving spectrograms to output path
- splitting of the generated spectrograms dataset into training and testing folders

[demo_gen_spectrograms.ipynb](https://github.com/dolphin-acoustics-vip/Spectrogram-Generator/blob/main/demo_gen_spectrograms.ipynb): This jupyter notebook is a sort of playground for testing and playing with different librosa functions and normalisation techniques on a sample waveform clip. This is not production ready code. A sample.wav has been provided in this repo for testing and experimentation, but the user can play with their own waveform data as well.

## Example spectrograms:
![Bottlenose](https://user-images.githubusercontent.com/71788619/162578789-f9231aa8-bd39-43d3-9215-8555e9c877d8.png) 
Normalized Bottlenose Wavclip

![Common](https://user-images.githubusercontent.com/71788619/162578829-4b024873-915a-43e0-a91f-da3b0594c22a.png) 
Normalized Common Wavclip

![Melon-headed](https://user-images.githubusercontent.com/71788619/162578841-904a5d6e-f391-4c29-8d5b-a5466d261bcc.png) 
Normalized Melon-headed Wavclip


