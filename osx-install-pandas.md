### Our recommendation

Anaconda CE is a simple installer that provides a Python installation with great number of data processing tools bundled.

For the purposes of this workshop, we recommend you download and install that package.

Then we will download the latest version of pandas and configure it to work with Anaconda Python.

### Download

Click this link, permitting your web browser to save it to the default location (which is probably ~/Downloads):

* http://09c8d0b2229f813c1b93-c95ac804525aac4b6dba79b00b39d1d3.r79.cf1.rackcdn.com/AnacondaCE-1.2.1-MacOSX-x86_64.sh

### Install

Open up a Terminal, and type these commands:

<pre>
cd Downloads
sh AnacondaCE-1.2.1-MacOSX-x86_64.sh
</pre>

Follow the prompts, and permit it to install. If you have questions, ask a staff member.

### Download pandas

In a terminal, run these commands:

<pre>
cd ~
mkdir -p projects
cd projects
git clone https://github.com/pydata/pandas.git
</pre>

This will download the latest version of pandas to your projects folder, creating it if necessary.

### Build pandas

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

# Back to laptop setup

[&laquo; Back to laptop setup](laptop setup)