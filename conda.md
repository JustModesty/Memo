1.list conda environment
  conda info --env
2.activate an enviroment
  conda activate <python-environment-name>
3.What is difference between pip 、conda and virtual environment?
  [this help](https://docs.conda.io/projects/conda/en/latest/commands.html#conda-vs-pip-vs-virtualenv-commands)
4.How to active conda in zsh?
  step 1: find the ".zshrc" file, and then vim it.
  step 2: export PATH=$HOME/miniconda3/bin:$PATH
  step 3: source .zshrc
  step 4: input conda --version in terminal,it will return the version if it works.

  Warning:In step 2,the path need to be the positon of miniconda3/miniconda/anaconda/anaconda3 or any other directory..
	  this path could be different each other. By default,the directory is in the $HOME.
