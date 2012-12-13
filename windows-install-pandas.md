## Our recommendation

On Windows, to get Pandas running, you have to install NumPy first.

To install NumPy:

* Click and download http://pypi.python.org/packages/2.7/n/numpy/numpy-1.6.1.win32-py2.7.exe
* Run the installer, and follow the process to the end.

Then, to install Cython:

* Click and download http://www.lfd.uci.edu/~gohlke/pythonlibs/ehdya7tk/Cython-0.17.2.win32-py2.7.exe
* Run the installer, and follow the process to the end.

Finally, you should install a graphing library to generate visual charts:

* Click and download https://github.com/downloads/matplotlib/matplotlib/matplotlib-1.2.0.win32-py2.7.exe
* Run the installer, and follow the process to the end.

### Test it

To make sure the process worked, open up a Python interpreter prompt. You should
see this familiar prompt:

<pre>>>></pre>

In that prompt, type the following:

<pre>
>>> import numpy
>>> print numpy.__version__
</pre>

You should see it print '''1.6.1'''.

To make sure cython is installed properly, you can do something similar:

<pre>
>>> import Cython
>>> print Cython.__version__
</pre>

You should see it print '''0.17.2'''.

To make sure matplotlib is installed properly, type the following into the Python interpreter:

<pre>
>>> import matplotlib
>>> print matplotlib.__version__
</pre>

You should see it print '''1.2.0'''.

### Download pandas from git

Now for the exciting part: we'll download the latest version of pandas, and configure it to run on your system.

To do that, click Start->Run->Git->Git Bash.

In that prompt, type the following:

<pre>
mkdir -p ~/projects
cd ~/projects
git clone https://github.com/pydata/pandas.git
cd pandas
</pre>

With those commands, you are downloading the latest version of pandas.

Enter these commands to "build" it:

<pre>
python setup.py build_ext --inplace
python setup.py build
</pre>

Now, make sure it worked by running these commands:

<pre>
python
</pre>

In the Python prompt, type this:

<pre>
>>> import pandas
>>> print pandas.__version__
</pre>

You should see a version number starting with 0.10.

### Success!

Now you have a Python environment set up to do high performance numeric calculations (with NumPy), build extensions (with Cython), and generate data visualizations (with matplotlib)!

[&laquo; Back to laptop setup](laptop setup)
