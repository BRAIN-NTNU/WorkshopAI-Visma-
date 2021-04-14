<a href="https://www.brainntnu.no"><img src="https://i.imgur.com/S9pM24h.png" width=240 align="right"></a>
# Workshop AI med Visma

Workshop AI med Visma og BRAIN NTNU - Februar 2021

## Setup

### Python

We will use Python for the Workshop. 

The easiest way to install python is probably from <a href="https://www.python.org/">here</a>
Hover the “downloads” tab, and then select “Windows”, “Mac OS”, or “Other Platforms” depending on your operating system. 

From here, you should select the latest stable installer for download (Python 3.9.2 at the time of writing). Click the downloaded package and follow the instructions to install python. 


### Pip

If you have a newer version of Python3, you probably already have “pip” installed. 
If you are uncertain whether or not pip is installed on you computer, you can run the following command on your mac/unix system terminal:
>> python -m pip --version

Likewise, you can check your windows system for pip by running the following command in your cmd:
>> py -m pip --version

If you have pip installed, you should see something like:
>> pip X.Y.Z from ...\site-packages\pip (python X.Y)

Note that if you have several versions of python installed on your computer, you might need to run 
>> pythonX -m pip --version

or

>> pyX -m pip --version

to instruct what version (X) of pip you are checking for. 

If you do not have pip installed, you should be able to install pip easily by following the instructions inder “installing with get-pip.py” for your operating system <a href="https://pip.pypa.io/en/stable/installing/">here</a>


### Python Libraries

You will also need some python libraries to help you with the optimization-task on the Workshop. 

You can install these easily with pip, just run the following commands one by one in your shell (terminal/cmd) of choice:
1. pip install ortools
2. pip install gmaps
3. pip install googlemaps
4. pip install geopy
5. pip install numpy
6. pip install matplotlib

Again, should there be some trouble with the installment that you can’t overcome for some reason, feel free to reach out for help. 


### Install Jupyter Notebook

We are using Jupyter Notebook for the Workshop as well:

<a href="https://jupyter.org/#:~:text=The%20Jupyter%20Notebook%20is%20an,machine%20learning%2C%20and%20much%20more."><img src="https://i.imgur.com/MmxC3mq.png"></a>

Download Jupyter Notebook (official tutorial [here](https://jupyter.org/install.html)):

1. Install with pip: `pip install notebook`
2. Verify successful installation with: `jupyter notebook`
3. End session: Press `cmd`+`C` on Mac, or `ctrl`+`C` on Windows.


## The Task 

The task for the Workshop will be to use optimization to find the best (most efficient) route for distributing COVID-19 vaccines to a list of adresses in Trondheim, Norway. 

### Google Distance API & Distance Matrix
In order to easily evaluate our routes, we need a quick way to get distances and expected driving-time between different points on a map. To do this, we will use the Google Distance API. In order to use this, you will need to create a (free) user on googles developers site to obtain an API key. However, for the sake of this workshop, if you do not want to create your own user, we have provided a copy of the distance matrix you will get from the API (distance_matrix.txt). 

Du kan enkelt importere denne som en numpy-array i python ved å kjøre følgende kodesnutt: 
>>import pickle
>>filehandler = open('distance_matrix.txt', 'rb') 
>>distance_matrix = pickle.load(filehandler)

### Solving the optimization problem 
If you have not done so by now, you can open the task-file (Brain.ai Workshop tasks.ipynb) in jupyter notebook. 
This will take you trough all the steps of solving the task, including: 
1. Creating a baseline solution
2. Solving the task with a genetic optimization algorithm 
3. Solving the task using Google Optimization Tools

You will see that we have provided a pretty thorough frame for all the code that you'll need to write, so you'll hopefully find it easy to follow the task from start to finish. Note however, that this is just one way of doing things - there are many more! So if you want to go completely rougue and write all the code for yourself, thats fine too! 

### Proposed Solution 
In "Brain.ai Workshop solution.ipynb" you will find a proposed solution for the Workshop! Feel free to compare your code with our approach. But do keep in mind that there are many ways to do things, so just because your could deviates from ours, doesn't mean it's any worse. It could even be better!

### Extra Challenges
At the bottom of the task-sheet you will find a list of extra challenges that might be fun to do if you like the task! 
We have, however, not made proposed solutions for these tasks. 

### HAVE FUN!
#### BRAIN NTNU & VISMA



