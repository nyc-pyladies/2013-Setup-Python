### Create an account on github.com

In order to conclude this process, you need to have an account on github.com.

Go to https://github.com/ and go through the signup process. We'll wait.

### Log in on github.com

Visit https://github.com/ and log in to the site.

### Visit the pandas project and "fork" it

The most convenient way to create and share changes on Github is by creating a *fork* of a project. In this fork, you may make whatever changes you want. When you're ready to request review of those changes, that is a separate process.

To make the fork, go to:

* https://github.com/pydata/pandas

Click the "fork" word in the top-right corner.

Finally, you should 

### Update your own computer to refer to that new fork

Open up the terminal program appropriate for your platform:

* On Windows, choose "Git Bash": click Start->Programs->Git->Git Bash
* On OS X, choose Terminal
* On a Linux system, choose gnome-terminal or your favorite terminal

Within that, type these commands:

<pre>
cd ~/projects
cd pandas
</pre>

This should put you in the project directory for pandas. The next commands we will type affect where git looks for updated versions of the pandas code.

This first set of commands renames the main project to be called "upstream":

<pre>
git remote rm origin
git remote add upstream https://github.com/pydata/pandas.git
</pre>

Finally, you will add your new fork as "origin". To do that, you will need to know your Github username.

Type the following command in:

<pre>
git remote add origin https://github.com/GITHUB_USERNAME/pandas.git
</pre>

To make sure it worked, type the following command:

<pre>
git fetch origin
</pre>

If it prints either nothing, or an informative message, then you are golden!

If you get an error message, do talk to a staff member.

# Back to laptop setup

[&laquo; Back to laptop setup](laptop setup)