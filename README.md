# Prerequisites:

For Handson Session you can choose any of the below platform (Anaconda or Google Colab)

## Anaconda 
1. Installation
#### Anaconda in Windows
Follow instructions in the below link to install Anaconda in Windows.
https://docs.anaconda.com/anaconda/install/windows/
#### Anaconda in Linux
Follow instructions in the below link to install Anaconda in Linux.
https://docs.anaconda.com/anaconda/install/linux/

2. Launch Anaconda Navigator. Go to Environments tab and click ‘Create’.

3. Input your environment name, e.g ‘dl_workshop’. Then click on ‘Create’, The pop-up window will appear, Select Python 3.7  and create. 
4. In the ‘dl_workshop’ environment, select ‘Not installed’ and search for ‘tensorflow’. Tick ‘tensorflow’ and ‘Apply’. The pop-up window will appear, click on apply. 
5. At your new ‘dl_workshop’ environment. Select ‘Not installed’ and search for ‘keras’. Tick ‘tensorflow’ and ‘Apply’. The pop-up window will appear, click on apply. 

6. Click on home, Install and Launch Jupyter notebook and run below code to verify your installation. Jupyter notebook Quick Start Guide: https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html#executing-a-notebook

```python

import tensorflow as tf
from tensorflow import keras
model_MLP = keras.models.Sequential()
model_MLP.add(keras.layers.Dense(units = 5 , activation = 'relu' ,input_shape = [4,]))
model_MLP.add(keras.layers.Dense(units = 1 , activation = 'sigmoid' ))
model_MLP.summary()

```

## Google Colab

Sign into Google account and visit below link
https://colab.research.google.com/#create=true

Run below code to verify your output.

```python
import tensorflow as tf
from tensorflow import keras
model_MLP = keras.models.Sequential()
model_MLP.add(keras.layers.Dense(units = 5 , activation = 'relu' ,input_shape = [4,]))
model_MLP.add(keras.layers.Dense(units = 1 , activation = 'sigmoid' ))
model_MLP.summary()
```
