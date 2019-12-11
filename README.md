# PowerBi-with-Py

Power Bi encounters
 issues importing packages with Py versions 3.6 and 3.7.

 

I was able to get around the error by creating a new conda env with Python 3.5:

jupyter notebook - new terminal :

conda create -n py35 anaconda python=3.5

Then pip installing relevant packages (I had issues with PowerBI recognizing conda installs):

 
conda activate py35
pip install matplotlib
pip install pandas
pip install seaborn
 

After this is complete, you need to point PowerBI to the new env.

 
File -> Options and Settings -> Options -> Python Scripting

 
Then add the Path to your new Env. Mine looks like:

"C:\ProgramData\Anaconda3\envs\py35"

 
