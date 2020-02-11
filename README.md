# Introduction to Astronomical Data

I have been giving talks on similar lines for past ten years using IRAF. But
IRAF is now reaching its end. The official IRAF website itself declares that it
will no longer be maintained and new users or those starting new projects must
switch to alternatives such as Astropy and its affiliated packages. I needed to
give this same set of talks again and decided to try and make them independent
of IRAF.

## How to Run - Windows Users

- Download: [](https://repo.anaconda.com/archive/Anaconda3-2019.10-Windows-x86_64.exe)
- Go the location where the file has been downloaded and double click this file.
- Follow the instructions as required. The default path to which Anaconda may be installed may contain spaces in its name and this will be reported by the Anaconda installer. If this happens, just create a separate folder without any spaces in its name at a different location and use that folder for installing.
- Open the "Anaconda Powershell Prompt" and type the following commands.
- First, we will need a package called 'ccdproc' - this can be installed by typing the following command:

    conda install -c astropy ccdproc

- We will also need a package called 'photutils' which can be obtained by the following command.

    conda install -c astropy photutils

- We need to visualize images. First one is calle 'ds9', let us download it from http://ds9.si.edu/download/win64/SAOImageDS9%208.1%20Install.exe; locate it; double click and install it. Use the default path "C:\SAOImageDS9". If you change this for some reason, please note it down.
- Another viewer we will need is called 'ginga' - this is to make the task 'imexam' interact with the Python program to do some interactive analysis. To install this package.

    conda install -c astropy ginga

- Our task now is to install 'imexam' but this too suffers from a lot of problems - a) conda install does not like to install it, b) pip install hates it as well and c) the default installation candidate for imexam has bugs! Some bugs are fixed but not released and some bugs are not fixed at all! And our exercise will depend on this bug. For this reason, we need to install from a forked / modified copy of imexam. But this means a little more complication in the installation process.
- First install 'git'. Download it from: [](https://github.com/git-for-windows/git/releases/download/v2.25.0.windows.1/Git-2.25.0-64-bit.exe). Then double click, accept all defaults and install it. You will have to restart your "Anaconda Powershell" for settings to take effect. This is important.
- In the newly restarted Powershell, type the following command:

    pip install git+https://github.com/vkaustubh/imexam.git

- How about we give things a spin? Let's see if Spyder is working. Go to Windows menu and search for Spyder and play with it.
- Next type the command "jupyter lab" from the Powershell and see if Jupyter Lab opens up. If it does, play around and close the browser window. And hit "Ctrl + c" in the powershell window to recover the prompt.
- Next up, for day 1 we are going to need some notebooks prepared for this workshop. For this, in your Powershell, give the following command.

    git clone https://github.com/vkaustubh/basic-astronomical-data.git
