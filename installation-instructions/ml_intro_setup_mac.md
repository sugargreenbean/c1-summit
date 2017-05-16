# Intro to ML: The Necessities
Source: https://github.com/DomenicPuzio

Note: these instructions are for Macs only

## Set up virtualenv
virtualenv allows you to keep dependencies required by Python projects in separate locations. Hence, you can keep different Python projects with different dependencies isolated.

First, install pip and virtualenv

`sudo easy_install pip
sudo pip install --upgrade virtualenv`

Now, create a virtualenv environment for Tensorflow.

`$ virtualenv --system-site-packages ~/tensorflow`

I placed mine in `~/tensorflow` but you can put it anywhere that makes sense. In the very least, I recommend that the lowest-level directory that you use is called `tensorflow`, but you do you, boo. This command will create the directory for you. You need to remember this location, so save it. On a sticky note, on the back of your hand, or maybe even as an environment variable in your .bash_profile for easy access in the future.

`export TENSORFLOW=~/tensorflow`

Now, we activate the environment by pointing to the activation script within our new directory.

`source ~/tensorflow/bin/activate`

Your prompt should now change to look like this:

`(tensorflow)$`

You are now inside the virtual environment!

## Install Tensorflow

`pip install --upgrade tensorflow`

## Install Jupyter notebook

`pip install jupyter`

From here, change to a directory where you would like your Notebook to be stored. Next, run the command to open up a Notebook editor. You can open specific Notebook files with this as well.

`jupyter notebook`

Congratulations! You're ready for the Summit!
