## List of Python packages used in the course

Note: Some of these packages have dependencies that will also need to be installed (and usually are installed automatically when you try to install the given original package).

### Included with Anaconda ([are all of these packages](http://docs.continuum.io/anaconda/pkg-docs.html))
* `ipython`
* `jupyter` (for notebook functionality)
* `matplotlib`
* `numpy`
* `pandas`
* `pip`
* `scikit-learn`
* `scipy`

### Available for installation via `conda` or `pip`
* seaborn (`conda install seaborn` or `pip install seaborn` depending on what you're using)
* pyparsing version 1.5.7 (`conda install pyparsing=1.5.7` or `pip install pyparsing==1.5.7` depending on what you're using)
* pydot (`conda install pydot` or `pip install pydot` depending on what you're using)

### Dude, what are my options if I don't want to install Anaconda?

#### If you don't want to use [Anaconda](http://docs.continuum.io/anaconda/), and you have a Mac:
* Get [Homebrew](http://brew.sh/) and follow the instructions for getting it at that link
* type `brew doctor` - fix any problems it tells you to fix (this might mean installing xcode command line tools, getting XQuartz, a bunch of other stuff)
* type `brew update`
* type `brew install python` in a terminal window (this will install pip, the package manager we want)
* individually install all of the packages you need listed above by following this pattern: `pip install BLAH` where BLAH is the package name.

#### If you don't want to use [Anaconda](http://docs.continuum.io/anaconda/), and you have a Linux Distro:
* Get pip-tools or pip (whatever it may be called on your distribution) via your favorite package manager (apt-get, yum, whatever)
* Use `pip` in the same way as the above Mac instructions to install the necessary packages

## In general, I recommend you install Anaconda. If you want to go down the path of installing the packages individually, you do so AT YOUR OWN PERIL.