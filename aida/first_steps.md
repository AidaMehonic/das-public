# Summary

In this project, my goal is to reproduce the entire repo: https://github.com/alan-turing-institute/das-public

Here, I will try to explain in detail everything I have had to do.

1. First, you need to install Python, R and the required packages. 
* The list of required Python packages is found here: https://github.com/alan-turing-institute/das-public/blob/master/requirements.txt
* The list of required R packages is found here: https://github.com/alan-turing-institute/das-public/blob/master/install.R

I used to have Anaconda on my laptop, but I decided I wanted to use plan Python for this project. 
I uninstalled Anaconda, and then installed the most recent Python version (currently 3.9.6).

Next, I pip installed all the required packages listed here: https://github.com/alan-turing-institute/das-public/blob/master/requirements.txt .

At this point, it seemed like I had everything needed to start reproducing the code.

So I cloned the repo to my GitHub Desktop. 

I tried to run parser_main.py - but I quickly ran into problems with logging. 

...

Just some quick notes here:
[] FTP downloads a tar.gz file which needs to be extracted first
[] In Windows 10, this can be done using this command: https://pureinfotech.com/extract-tar-gz-files-windows-10/
[] I want to start by creating a small set of articles in a folder called dev_set in DAS_public/dataset
[] dev_set is created by running sample_dev_set.py --- NOTE: You will need to manually edit line 9 to edit your root folder 
