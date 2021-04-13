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

Note that if you have several versions of python installed on your computer, you might need to run “python3 -m pip --version” or “py3 -m pip --version” to instruct what version of pip you are checking for. 

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

