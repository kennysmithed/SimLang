# [Simulating Language 2020](https://github.com/kennysmithed/simlang)

This is a collection of interactive notebooks for a course taught in the [Centre for Language Evolution](http://lel.ed.ac.uk/cle) at Edinburgh showing how to model the evolution of language at all timescales - from individual utterances, through individual learning, cultural transmission, and biological evolution. This course covers many of the major research breakthroughs over the past two decades, and shows how easy it is to build simulations of language evolution. It is suitable for anyone, even without any background in coding, and uses only a very basic subset of the programming language, Python, throughout.

## Using the interactive notebooks

The interactive Python notebooks work using a "Jupyter Server". The University of Edinburgh provides one that you can log into here: https://noteable.edina.ac.uk/login

<!--Alternatively, if you're not a student at the University of Edinburgh, you can use Binder to interact with the notebooks on a temporary free server: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/kennysmithed/simlang/master)
-->

If you're using the noteable service you'll need to download the files onto the server. Once you've logged on to the noteable service you may have to either "reconnect" or "start" your server (if there is a list of options available, stay with "standard notebook"). Once you've done that you'll be given an interface that will let you upload notebooks and navigate the files you'll be creating. First, we need to upload the notebooks from this github site. To do that, you need to open a new notebook that you'll use to update the files regularly (whenever a new notebook is posted for example). Follow these steps:

- Click on the "new" menu.
- Select "Python 3". This will open a brand new notebook.
- In the first "cell" of the notebook, you need to enter some code that will handle the transfer from the github site.

Copy and paste the following code into the cell:

	!rm -rf simlang
	!git clone https://github.com/kennysmithed/simlang
	!mkdir -p simlang_local
	!cp -nr simlang/* simlang_local


- Run this code by pressing SHIFT + ENTER. This will transfer all the current simlang content into your notebook server. It also makes a "local" copy of the code in a folder called "simlang_local". This is the one you should do your work in, safe in the knowledge any changed you make won't get overwritten.
- Rename your notebook something like "Update Course" by clicking on the "file" menu and then "rename"
- Save the notebook by clicking "file" and then "save and checkpoint".

Now you're done. You can close that browser tab. Next time you want to add new notebooks from the course website, just open the notebook "Update Course.ipynb" in the file list in the first noteable window and run that first cell again by pressing SHIFT + ENTER.

You can now click on the "simlang_local" folder in the file list in the noteable window and open any of the notebook files that are there. If you mess anything up, you can delete the notebook you're working on, run the update course notebook again and you'll have a fresh file to work from. (But be careful, you won't be able to undo this!)

[Kenny Smith](http://lel.ed.ac.uk/~kenny/), University of Edinburgh, 2019

The following files are copyright (c) 2009-2019 [**Simon Kirby**](http://www.lel.ed.ac.uk/~simon), with contributions from [Kenny Smith](http://www.lel.ed.ac.uk/~kenny/), [Jennifer Culbertson](https://jennifer-culbertson.github.io), [Andrew Smith](https://www.stir.ac.uk/people/256435): lab1.ipynb, lab1_answered.ipynb, lab1_walkthrough.ipynb, lab1_notebook_intro.ipynb

The following files are copyright (c) 2020 [**Kenny Smith**](http://www.lel.ed.ac.uk/~kenny), with contributions from [Simon Kirby](http://www.lel.ed.ac.uk/~simon): lab2.ipynb, lab2_answered.ipynb, lab3.ipynb

All aspects of this work aside from the Software itself is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). For Software license, see [LICENSE file](LICENSE) for items copyright Simon Kirby, and [LICENSE file](LICENSEKS) for items copyright Kenny Smith.
