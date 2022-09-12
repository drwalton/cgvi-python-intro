# CGVI Introduction to Python 2021

## Quick Start

Use the following links to open each of the notebooks for this session in Google Colab, and run them straight away in your browser:

* [00: Introduction](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/00_introduction.ipynb)
* [01: Variables and Operators](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/01_variables_and_operators.ipynb)
* [02: Data Structures](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/02_data_structures.ipynb)
* [03: Control Flow](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/03_control_flow.ipynb)
* [04: Numpy](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/04_numpy.ipynb)
* [05: Matplotlib](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/05_matplotlib.ipynb)
* [06: Images](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/06_images.ipynb)
* [07: Linear Algebra](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/07_linear_algebra.ipynb)
* [08: Randomness & Probability](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/08_randomness_probability.ipynb)
* [09: Loading & Saving](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/09_loading_saving.ipynb)
* [10: Differentiation & Gradient Descent](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/10_differentiation.ipynb)

This repository contains jupyter notebook files for the CGVI python induction. Each of these notebooks contains a mixture of blocks of code and text. 

You can run and edit the code yourself, and I strongly encourage doing so to better understand how it works.

Many of the notebooks contain exercises. These won't be marked but completing them will also deepen your understanding of the material covered here, and should help to prepare you for your other modules. Solutions for these exercises are available in the `solutions` directory, and can be opened in Google Colab through these links:

* [01: Variables and Operators](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/01_variables_and_operators.ipynb)
* [02: Data Structures](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/02_data_structures.ipynb)
* [03: Control Flow](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/03_control_flow.ipynb)
* [05: Matplotlib](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/05_matplotlib.ipynb)
* [06: Images](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/06_images.ipynb)
* [07: Linear Algebra](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/07_linear_algebra.ipynb)
* [08: Randomness & Probability](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/08_randomness_probability.ipynb)
* [09: Loading & Saving](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/09_loading_saving.ipynb)
* [10: Differentiation & Gradient Descent](https://colab.research.google.com/github/drwalton/cgvi-python-intro/blob/main/solutions/10_differentiation.ipynb)

## Notebook Contents

Each of the notebooks will introduce a series of concepts in python that will be useful for your CGVI course. The contents of the notebooks are as follows:

* 00: Introduction:
    * Brief introduction to Jupyter notebook, and how to run code.
* 01: Variables and Operators:
    * Introduction to creating and using variables, and operators (e.g. `=`, `*`, `+` and so on).
* 02: Data Structures:
    * Structures for storing larger amounts of data, including the list, dict and tuple.
* 03: Control Flow:
    * Managing control flow with loops, and organising code into functions.
* 04: Numpy:
    * Introduction to the numpy library and its array data structure.
* 05: Matplotlib:
    * Introduction to the useful graph-plotting library Matplotlib.
* 06: Images:
    * Introduction to the `cv2` image library, and processing image files.
* 07: Linear Algebra:
    * Using `numpy` to perform some linear algebra operations.
* 08: Randomness & Probability:
    * Using `numpy.random` to generate data following random distributions, and looking at conditional probability.
* 09: Loading & Saving:
    * Loading and saving text files, handling exceptions, saving numpy arrays to file.
* 10: Differentiation & Gradient Descent:
    * Different ways to differentiate functions in numpy, gradient descent, autodiff in `pytorch`.

## Running the Notebooks

To view these files, you can click on the links for each file above. This will show you the notebooks themselves, along with the outputs produced when I ran them. However, you won't be able to run the code.

To run the code you will need to open a Jupyter server. The quickest way to do this is to use Google Colab.

### Colab

Google Colab is a service where Google will host the Jupyter server and run the python code for you on their servers, so you can get started straight away without having to install python.

To do this, open [Google Colab](https://colab.research.google.com). Click on File->Open if you need to, then select the Github tab. Enter the name of this repository, `drwalton/cgvi-python-intro` and you can then select the notebooks for this introduction below.

Alternatively, you can follow the direct links at the top of the page.

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

## Contact

If you run into issues with these notebooks, or find an error in the code, please let me know. You can file an issue on this github repository (go to the Issues tab at the top of the page, and then click the "New Issue" button) to highlight any specific issue with the code. This will be publically viewable. If you would prefer to contact me directly, please do so at `david.walton.13 at ucl.ac.uk`
