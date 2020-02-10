# Introduction to Astronomical Data

I have been giving talks on similar lines for past ten years using IRAF. But
IRAF is now reaching its end. The official IRAF website itself declares that it
will no longer be maintained and new users or those starting new projects must
switch to alternatives such as Astropy and its affiliated packages. I needed to
give this same set of talks again and decided to try and make them independent
of IRAF.

## How to Run?

Since I generally anticipate participants from diverse backgrounds, I generally
ask them to use the Anaconda distribution. Assuming you are using the latest
Anaconda distribution and you are in an Anaconda shell, you can install the
additional packages needed by saying,

    $ pip install ccdproc imexam photutils ginga

And then from the folder where you have downloaded this repo, start Jupyter Lab
by saying,

    $ jupyter lab

And that should be sufficient.

__Note__: Windows users are likely to suffer because of overall lack of native
libraries and other things. Special instruction set for them coming up soon.
