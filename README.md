[<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/81/Ernest_Solvay.jpg/164px-Ernest_Solvay.jpg" align="right">](https://en.wikipedia.org/wiki/Ernest_Solvay)
# solvay-nb
UJI Solvay Notebooks allows you to execute [jupyter notebooks](https://jupyter.org/index.html)
in the central node (solvay.uji.es) of [UJI's high-performance
computation cluster](http://www.uji.es/serveis/si/serveis/calcul/recal/).

# Installation
1. You need an account at the cluster solvay ([form](https://e-ujier.uji.es/pls/www/!gri_ass.spi020102?p_proc=251&p_tema=12)). 

2. Clone the repo into your solvay account with:

`$ git clone https://github.com/ecervera/solvay-nb.git`

3. Add the following lines to your `.bashrc` file:

`export PATH="/usr/local/octave/bin:$PATH"`

`export PATH="/usr/local/conda/miniconda3/bin:$PATH"`

`export PYTHONPATH=`

# Execution (macOS / Linux)
1. In your desktop or laptop computer, run in a terminal:

`$ ssh -L 8888:localhost:8888 solvay -t "jupyter-notebook --no-browser --notebook-dir=solvay-nb"`

2. In your browser, open the URL displayed in the terminal.

3. Open the `INDEX.ipynb` file.

# Execution (Windows)

You need [PuTTY](http://www.putty.org/) installed in your computer.

1. In your desktop or laptop computer, open a Windows console and run:
`plink -ssh solvay -L 8888:localhost:8888 "jupyter-notebook --no-browser --notebook-dir=solvay-nb"`

2. In your browser, open the URL displayed in the terminal.

3. Open the `INDEX.ipynb` file.
