## First, install dependencies

Pandas requires a number of other Python libraries to be installed. To install them, if you are running Debian or Ubuntu, run the following command:

<pre>sudo apt-get install python-numpy cython</pre>

This will instal a fast numeric processing library (numpy) and a tool required in the pandas build process (cython).

# Test numpy

Open up a Python prompt by running the following:

<pre>python</pre>

At the prompt, type the following:

<pre>
 >>> import numpy
 >>> print numpy.__version__
</pre>

You should see a number like "1.6.1" or higher. If you see an older version, like "1.5.1", you need to get help from a staff member to set up a "virtualenv."

# Test cython

Open up a Python prompt by running the following:

<pre>python</pre>

At the prompt, type the following (capitalization matters!):

<pre>
 >>> import Cython
 >>> print Cython.__version__
</pre>

You should see a number like "0.15.1" or higher. If you see an older version, like "0.14.1", you need to get help from a staff member to set up a "virtualenv."

# Download pandas

We recommend storing pandas in a directory called ''projects'' in your user directory. To do that, run the following commands:

<pre>
mkdir -p ~/projects
cd ~/projects
git clone https://github.com/pydata/pandas.git
cd pandas
</pre>

You will see git download pandas. Once the download finishes, and you get your prompt back, proceed to the next step.

# Installing Pandas inside the VirtualEnv
Alternatively, if you would like to create a development sandbox environment, we recommend installing Pandas inside the VirtualEnv. Instructions to create a virtualenv are here: [http://virtualenvwrapper.readthedocs.org/en/latest/command_ref.html](http://virtualenvwrapper.readthedocs.org/en/latest/command_ref.html)

Next, you must 'cd' (change directory) into the '/Env' located in /path/to/home/. To do that, run the following commands:
<pre>
cd Envs/
export WORKON_HOME=~/Envs
mkdir -p $WORKON_HOME
mkvirtualenv pandas
</pre>
Then, 'cd' into the '/pandas' directory and follow the installation instructions on this page: [http://pandas.pydata.org/pandas-docs/stable/install.html](http://pandas.pydata.org/pandas-docs/stable/install.html)
You will need to install all the dependencies inside the Env.


# Build pandas

To build pandas, you have to run the following two commands:

<pre>python setup.py build_ext --inplace</pre>

This will take about 2 minutes. Once it is finished, run this command:

<pre>python setup.py build</pre>

This will also take about 2 minutes.

# Test pandas

To make sure it has built properly, run the following command inside the pandas directory:

<pre>python</pre>

Within this python prompt, type:

<pre>
 >>> import pandas
 >>> print pandas.__version__
</pre>

You should see this version number: '''0.10.0b1'''. If you see something different, get help from an instructor.

# Install ipython

''ipython'' is an enhanced interactive Python shell that will be used during the lecture. To install it, run:

<pre>sudo apt-get install ipython</pre>

# Back to laptop setup

[&laquo; Back to laptop setup](laptop setup)

