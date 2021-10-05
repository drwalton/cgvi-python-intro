# CGVI Introduction to Python 2021

This repository contains jupyter notebook files for the CGVI python induction. Each of these notebooks contains a mixture of blocks of code and text. 

You can run and edit the code yourself, and I strongly encourage doing so to better understand how it works.

## Getting Started

To view these files, you can click on the links for each file above. This will show you the notebooks themselves, along with the outputs produced when I ran them. However, you won't be able to run the code.

To run the code you will need to open a Jupyter server. The quickest way to do this is to use Google Colab.

### Colab

Google Colab is a service where Google will host the Jupyter server and run the python code for you on their servers, so you can get started straight away without having to install python.

To do this, open [Google Colab](https://colab.research.google.com). Click on File->Open if you need to, then select the Github tab. Enter the name of this repository, `drwalton/cgvi-python-intro` and you can then select the notebooks for this introduction below.

Alternatively, you can follow the direct links here:

* [00: Introduction](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/00_introduction.ipynb)
* [01: Python](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/01_python.ipynb)
* [02: Numpy](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/02_numpy.ipynb)
* [03: Matplotlib](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/03_matplotlib.ipynb)
* [04: Images](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/04_images.ipynb)
* [05: Linear Algebra](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/05_linear_algebra.ipynb)
* [06: Randomness & Probability](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/06_randomness_probability.ipynb)
* [07: Loading & Saving](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/07_loading_saving.ipynb)
* [08: Differentiation & Gradient Descent](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/08_differentiation.ipynb)

If you are logged into your Google account, you should be able to modify the notebooks and save them to your Google Drive if you would like to.

**Warning:** Please note that [computational resources on the free version of Google Colab aren't unlimited](https://research.google.com/colaboratory/faq.html#resource-limits). This shouldn't be an issue for running fairly lightweight code like this tutorial, but if you are running intensive GPU-based machine learning code for coursework, for example, there's a risk you may "run out" of compute at an unfortunate time. Even the [paid versions of Colab (Pro and Pro+)](https://colab.research.google.com/signup) do not absolutely guarantee resources will always be available. If you have access to a good computer, it may be worth the time setting up a local server to get guaranteed compute resources.

### Running a Local Server

Running a local notebook server gives you more control over your setup, but takes some work to get up and running. To run it you will need to install python, and then a number of required libraries. The best way to do this will depend on your computers Operating System (see instructions below).

Once you have everything installed, you can type `$ jupyter notebook` into a terminal. This will start a local jupyter notebook server, and open a page in your web browser. From here you can select the `.ipynb` notebook file you would like to view.

These notebooks can also be opened using [Visual Studio Code](https://code.visualstudio.com/) with the [jupyter notebook extension](https://code.visualstudio.com/docs/datascience/jupyter-notebooks), but this also requires that you have python and jupyter installed locally.

#### Linux

In Linux, it is probably easiest to install the most recent version of python and pip using your distribution's package manager. On Debian/Ubuntu, this would be:

`$ sudo apt-get install python3 python3-pip`

Note that if you are using a different distribution both the command and package name may be different, please look up the correct command for your distro.

Now you can install the required packages:

`$ pip3 install numpy matplotlib opencv-python jupyter`

#### Windows

On Windows I have had most success using [Anaconda](https://www.anaconda.com/products/individual).

Once this is installed, you can open up an anaconda terminal from Start Menu -> Anaconda3 -> Anaconda Powershell Prompt.

Here you can install the required packages with:

`$ conda install numpy matplotlib jupyter opencv`

#### Mac

Anaconda is also available for Mac, and once installed, the packages can be installed in the same way as described for Windows above.

Alternatively, python and pip can be installed using a package manager - two popular options are [Homebrew](https://brew.sh/) and [MacPorts](https://www.macports.org/).

Once you have installed python and pip using the package manager of your choice, you can then install the packages with:

`$ pip3 install numpy matplotlib opencv-python jupyter`

### Pytorch

The final examples in the differentiation notebook use Pytorch. If you're running a local Jupyter server I'd recommend installing pytorch following the [guide here](https://pytorch.org/get-started/locally/).

The examples here do not use GPU, so installing the CPU-only version of pytorch will work fine. 

For Mac OS users, the CPU-only version is the only one available pre-compiled. It is possible to build pytorch from source, but I have not tried this, and CUDA support on Mac OS is limited, so I'm not sure I'd recommend it. If you have a Mac with an Nvidia GPU, you can alternatively install Windows via [Boot Camp](https://support.apple.com/en-gb/boot-camp) and then install pytorch with GPU support (but this will require a licensed copy of Windows).
