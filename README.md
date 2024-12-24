Digital Signal Processing Courseware: An Introduction (copyright © 2024)  
Authors: J. Christopher Edgar and Gregory A. Miller

# Digital-Signal-Processing-Courseware

## Course Goals and Content

This courseware is written for an audience that does digital signal processing (e.g., people who do neuroscience) but that do not have a strong math or engineering background. The goal of the course is that after you have completed the book you'll have a fairly sophisticated understanding of how to apply several digital signal processing techniques, including better understanding what is really happening when you push certain buttons in packaged neuroimaging software (e.g., filter settings). After completing the book you'll also better understand how to collect neuroimaging data (e.g., data sampling rate).

Each Lesson in the Digital Signal Processing courseware contains four sections: Basics, Tutorial, Give It a Try, and Literacy. The Basics section should be read first, as this section covers the primary topic. The Basics section is followed by the Tutorial section, and this section expands upon what is presented in the Basics. Having completed the Basics and Tutorial sections, you then have the opportunity to more deeply encode what you've learned by completing the Give It a Try Try (providng answers in the electronic document) and the Literacy section (perhaps printing and answering using pen and paper).

The courseware covers the following topics:  

**Lesson 1** Introduction to sine/cosine functions, discussion of time series and spatial data, discussion of amplitude, frequency, and phase, and a section on adding sine waves. There's also a brief introduction to complex numbers and the Euler Identities. Students also read in time and spatial data (grayscale images).

**Lesson 2** Detailed discussion of the Nyquist Theorem and aliasing (time and spatial domain), a section on multiplying sine waves, and a brief discussion of plotting complex numbers and determining the magnitude and phase of complex numbers.

**Lesson 3** This lesson focuses on convolution, and via convolution, filtering. Ideas are explored in the time domain. In this process, students are introduced to high- and low-pass filters and gain functions.

**Lesson 4** Generally the same as Lesson 3, but now examining spatial data. Students use convolution methods to filter grayscale and color images. Normal distributions and random noise are also discussed.

**Lesson 5** This lesson focuses on using sine and cosine to compute the magnitude and phase of activity at different frequencies: time and spatial data. Students also see that magnitude and phase information can be obtained more easily using complex exponentials.

**Lesson 6** The Fourier transform is finally introduced and some of the limitations (and ways to overcomesome of these limitations) of time-frequency transforms examined. Students are also introduced to the idea of filtering using forward and inverse Fourier transforms.

## Courseware - How to use

-For each lesson, be sure to do the modules in order: Basics, Tutorial, Give It a Try, Literacy.

-When you load each Jupyter Notebook *.ipynb file, select and run the first code cell (right after the “Setup” text cell). It runs some initialization code that later code will need, so do that before you run later cells.

-Jupyter Notebook can be thought of as an enriched text editor, providing local code execution, including display of graphical products of your code.

-In our experience, the commands available in the ribbon at the top of the Jupyter Notebook window vary a little across PCs, even when all are running Windows 10. We don’t know the extent of this variation or what it depends on. Accordingly, you may find some of the commands we suggest in a different dropdown menu and/or labeled a bit differently than what’s in our instructions. Feel free to explore the menus. For example, there may or may not be a “Cell” command in that ribbon. If not, there may be a number of cell commands under the Run button.

-Before starting the Lessons, make a backup copy of all the files we’ve provided. If a Lesson file stops working, you can always start again with a clean file from your backup. Also, in some files, we ask you to alter code, add code, or enter an answer to a question. You may want to retain an original copy that doesn’t have those changes.

-If you want to exit and later resume where you were in a Jupyter Notebook:

1) Make a note about where you are before you exit (e.g., that you finished DSP.01.B1.c, or that you’re ready to tackle the cell with the text “We need to consider a third and final aspect of a sine-wave timeseries”).
2) When you re-start that Jupyter Notebook, use ctrl-F to find that section, select that cell, and in the command ribbon at the top: click on Run | Run All Above Selected Cell. That way, any code that relies on earlier code having been run (executed) will have run before you more forward.
3) You’re welcome to edit our code and re-run a cell, for example to plot a different frequency. But note that changing the computation or even the value of a variable that’s used later in the file could lead to different outputs than our text narrative assumes.

-If your Jupyter Notebook Web page becomes generally or selectively unresponsive, try each of these, in this order:

1)	Reload the current Web page: hit your browser refresh button
2)	Click Kernel | Restart Kernel and Run up to Selected Cell [or equivalent in the menus available to you]
3)	Save your *.ipynb file (at least try to: ctrl-S or floppy-disk icon in command ribbon or File | Save Notebook in command ribbon), exit Jupyter Notebook entirely, and re-start

# Installing Anaconda

-Anaconda is a Web-browser-based environment for writing and running code. (Anaconda is also a commercial company that we understand provides Anaconda3 and its support for Jupyter Notebook for free to users like us. We have no affiliation with the company.) You can store Jupyter Notebook files (*.ipynb) on your local computer or wherever you want. 

-Some Web postings note that, at least on Windows, attempting to install Anaconda on a computer that has a previous Anaconda installation may fail and that the previous installation may be difficult to fully remove to clear the way for a new installation. https://docs.anaconda.com/navigator/uninstall/ provides uninstall instructions, but in our experience, and as noted in Web comments, that didn’t work. What worked for us involved: conventional uninstall of Anaconda3, manual removal of some leftover directories under C:\users\<username> per https://docs.anaconda.com/reference/troubleshooting/: scroll down to Files left behind after uninstalling Anaconda on Windows – we found and deleted some of the directories listed there plus a few more than seemed relevant; and manual cleanup in the Windows Registry – which is seriously risky to edit – don’t try if you’re not sure how to do that; if you choose to do it: we searched for and deleted all keys containing “anaconda”; we found none containing “jupyter”

-Install Anaconda3 on your computer per https://docs.anaconda.com/anaconda/install/. Accepting defaults should be fine. (The download for MacOS will include a choice between “Apple Silicon” and “Intel”. That refers to the type of CPU in your computer. Apple switched its Macs to Intel CPUs circa 2006 and then to Apple-designed M-class CPUs beginning in 2020.)

# Download the Jupter Notebook files

-From this GitHub page access the courseware files for Lessons 1 to 6

-You’ll use Jupyter Notebook files running in a Web browser, accessing files on your computer. Consider what Web browser you’ll use. We’ve tested with Firefox and Chrome on Windows 10 and Firefox on MacOS Ventura 13.2.1. If you want to use another browser, test it with our Jupyter Notebook files before the workshop.

-Consider what directory on your computer you want to download the files to.

-We aren’t aware of a way to set the default directory in Jupyter Notebook so that *.ipynb files load from a directory of your choice. But, after you launch Anaconda | Jupyter Notebook, you’ll be in your Web browser, and you can navigate to that directory within Anaconda to access those files – instructions below.

# Start a Session 

-On Windows, clicking Start | Anaconda3 |Jupyter Notebook opens a text box in which it runs commands, then opens a tab in your default Web browser at http://localhost:8888/tree (or similar) showing your directory tree under C:\users\[account name]\Documents\Jupyter, e.g. under C:\Users\gmiller\Documents\Jupyter. Either already you’ve copied our files to that directory, or… 

-…change to another directory, previously created, containing the *.ipynb file you want to open, per https://saturncloud.io/blog/jupyter-notebook-change-directory-a-comprehensive-guide/. For example, if you want to work within a directory you call MyDirectory:

1) Click New [upper right] | Terminal (opens a Windows Power Shell text box) | type “cd MyDirectory” (or paste in a text string of your desired directory – ctrl-V or right-click | Paste | Paste)
2) Then type “jupyter notebook”, which will run the command in that text box, then open a browser tab @ http://localhost:8888/tree (or similar) showing the directory tree under MyDirectory, e.g.: Click New | Terminal | cd MyDirectory
3) Jupyter Notebook will let you save the currently loaded file with a different filename, but only within the current directory  
 
-Navigate to the directory containing the desired *.ipynb Jupyter Notebook file and click on that file open it in another browser window.

-Case of text (upper case or lower case) in directory paths and filenames generally doesn’t matter in Windows but does matter in *nix-derived operating systems such as MacOS and Linux.

-Avoiding spaces (blanks) in directory names and filenames is highly advisable in some contexts, especially for work at the command line in Windows, MacOS, and Linux.

-Browser extensions that you may have installed, such as to enhance security or block ads, might block access even to a local directory. If you have trouble reaching your local directory, consider adjusting relevant settings or moving our files to another directory.

# Basic Navigation in Jupyter Notebook 

-You do need to know how to navigate the Jupyter Notebook user interface. It’s largely self-explanatory, and we intend to provide enough information here to get you going. But feel free to consult the short tutorial at https://learning.anaconda.cloud/get-started-with-anaconda?souce=installation-success.

-Our Jupyter Notebook files use Python code, but you don’t have to know anything about Python or other languages to use them.

-Sometimes we ask you to look briefly at a snippet of code. If you’re not familiar with Python, just look for something relevant at the moment, such as the ‘freq’ frequency variable or the ‘gain’ magnitude variable. 

-Here and there, we ask you to copy, paste, and/or edit a bit of Python code, for example to change the frequency or magnitude of a sine wave. Again, if you’re not familiar with Python, just look for something relevant at the moment, such as the ‘freq’ frequency variable or the ‘gain’ magnitude variable. Or grab a line of code from an earlier cell that does approximately what you want and edit it so that it does exactly what you want.

-For example, to plot an “A” character 90 degrees into the 1 Hz sine wave in the Lesson 1 Literacy notebook section L.5 (this will make sense when you get there), you can copy the nearby line of code: plt.text(1,0,'1 sec',fontsize=15) paste it into the code cell, and edit it to, for example: plt.text(.25,0,'A',fontsize=15). 

-Each Jupyter Notebook file opens in a Web browser page, with a command ribbon at the top and then a series of cells. Some cells will load as regular text, some as Python code. Each cell can be run separately (even text cells will run, but that just means: re-display as simple text after having opened the file for editing).

-Generally, you proceed through the cells in order. You can run a cell by typing shift-Enter.

-To select a cell, click on it.

-To edit a cell (whether text or code), double click on the cell.

-To get out of edit mode, type shift-Enter or click the ‘run’ button in the menu bar.

-In some cells, this will reveal code that presents text.

-You can run a series of cells in order by hitting shift-Enter repeatedly.

-But you don’t have to run cells in order – you can scroll back to an earlier cell. You can exit the notebook at any time, and you can re-load it and start over, or pick up where you left off, or anywhere else.

-If you want to resume at a particular place in the file, before you exit you may want to make a note about where you are (e.g., that you finished section DSP.01.B1.c, or that you’re ready to tackle the cell with the text “We need to consider a third and final aspect of a sine-wave timeseries”).

-When you re-start it, use ctrl-F to find that section, then in the command ribbon at the top: click on Run | Run All Above Selected Cell. That way, any later code that relies on earlier code having executed already will have run before you more forward.

-When you load a Jupyter notebook file and start working in it anywhere other than at the very  beginning, when you get to the cell you’re going to start with: Before you do anything else, it’s a good idea to:

1) Select that cell.
2) In the menu bar at the top of the browser window, click Run | Run All Above Selected Cell, to be sure that variables and other things have been defined. A common problem if you don’t do that is a “NameError” about an undefined variable. If you see that, back up a cell or two, click Run | Run All Above Selected Cell, and proceed to run each cell in order from there.
 
-We’ve found that the details of how to clear all output or exit vary a little on different PCs. To clear all output using the menu bar, these two alternative procedures worked on different PCs:

1) Click Cell | All Output |Clear
2) Click Kernel | Restart Kernel and Clear Outputs of All Cells… | Restart
 
-Reminder: run the first code cell (right after the “Setup” text cell) in of our Jupyter Notebook files. It runs some initialization code that later code will need, so do that before you run later cells.

-So be sure to run that initialization cell before you move on.
 
-There are several commands relevant to ending a session under the File option in the menu bar.  

-Click File | Close and Shut Down Notebook Ctrl+Shift+Q | OK

-Click File | Log Out or Shut Down

-It’s OK close browser the tab, the browser, and/or the Power Shell text box.


Originally written in Mathematica by J. Christopher Edgar. Conversion to Jupyter Notebook by Song Liu. The authors of this courseware are indebted to Prof. Bruce Carpenter (University of Illinois Urbana-Champaign). Bruce inspired the creation of this courseware, he consulted with the authors as this courseware was being developed, and he provided the original version of the code and text for several sections of this courseware (e.g. the section on complex numbers and the section on normal distributions). 



