Code: Jupyter Notebook format

The program is coded in Jupyter Notebook format, where the calculation results are recorded in the same location as the program.

First, install the application Anaconda [Win, Mac, or Linux] (https://www.anaconda.com/download) in your system.

After installation, open the Anaconda prompt and install joblib, a library for parallel computing, as follows: 
    conda install joblib

Now, in the folder where the above program is located, make a folder named fasta and save some of the FASTA files you want to analyze in it.

After you have installed Anaconda, you can launch the application Jupyter Notebook.

However, if you launch the app as is, it will select the notebook from the default location of your account. As this is inconvenient, I always start it from within the Anaconda prompt, and change directory to the location where the above program is located. Then,

    jupyter notebook --notebook-dir="."

This option --notebook-dir=**** means that the directory in which the command is executed will be changed to the "current directory".

If you want to do a frequency count, from the list of programs select the following file:

    count_Fasta_Window_Step_Size_Ver_2_2.ipynb

After the program opens, in the Parameter Settings, change the following parameters:

    nuc_length
    window_size
    step_size
    others_th
    trim_rule 

Then, go to the top menu and follow these steps:

    Kernel → Restart & Clear Output
    Cell → Run All

The pattern count will start.

After the pattern counting is completed, SOM analysis is performed based on the frequency information.

Return to the list of programs to open the SOM program:

    Batch_SOM_for_Nucleotides_Ver_8_4.ipynb

As mentioned above, set the various parameters and then select the following commands from the menu at the top:

    Kernel → Restart & Clear Output
    Cell → Run All

The SOM analysis will start; when it finishes, you will find the analysis results in the fasta folder.
