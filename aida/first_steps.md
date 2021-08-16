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
* FTP downloads a tar.gz file which needs to be extracted first
* In Windows 10, this can be done using this command: https://pureinfotech.com/extract-tar-gz-files-windows-10/
* I want to start by creating a small set of articles in a folder called dev_set in DAS_public/dataset
* dev_set is created by running sample_dev_set.py --- NOTE: You will need to manually edit line 9 to edit your root folder 

...

Now some notes on MongoDB:

1. You need to first run MongoDB. In the Windows Command Prompt, you would do this by typing the command: mongod.exe "--dbpath c:\data\db". 
2. Do make sure that the folder c:\data\db already exists before you run the command.
3. After mongod.exe has run successfully, open MongoDB Compass.
4. Connect to the mongod service you are running by specifying:
   * hostname: localhost
   * port: 27017   


NOTE: If you try to run mongod.exe without first creating the folder where you want to store your data (for instance c:\data\db), MongoDB Compass will not connect properly.

...

You need to have MongoDB running before you can run parser_main.py. 
