
## Project Overview

This is my work for Convolutional Neural Networks (CNN) project in the AI Nanodegree. In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  


### Instructions

I would like to give you instructions before you use my notebook. These are config steps if you are using AWS EC2 instance. You should have connected to your EC2 and configured jupyter before following steps.

1. Clone the repository and navigate to the downloaded folder.
```	
git clone https://github.com/udacity/dog-project.git
cd dog-project
```

2. Download the dog dataset using `wget https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip`.  Unzip the folder at location `path/to/dog-project/dogImages`. 

3. Download the human dataset using `wget https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip`.  Unzip the folder at location `path/to/dog-project/lfw`.

4. Donwload the VGG-16 bottleneck features using `wget https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz` for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`. You might need other structures in the transfer learning practice. Feel free to use similar command and place them in the same folder.
	
5. **If you are using AWS**, install Tensorflow.
```
sudo python3 -m pip install -r requirements/requirements-gpu.txt
```
	
6. Switch [Keras backend](https://keras.io/backend/) to TensorFlow. 
```
KERAS_BACKEND=tensorflow python -c "from keras import backend"
```
7. Run jupyter, and it will print out a url in the session. Then open your browser, and paste the url with `X.X.X.X:8888`. `X.X.X.X` is your EC2 instance IP, then use 8888 instead of 0000 and paste your token. You should have your notebook open.
```
jupyter notebook --ip=0.0.0.0 --no-browser
```
