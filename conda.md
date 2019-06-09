## 1.list conda environment

  conda info --env

## 2.activate an enviroment

  conda activate <python-environment-name>

## 3.What is difference between pip 、conda and virtual environment?

  [this help](https://docs.conda.io/projects/conda/en/latest/commands.html#conda-vs-pip-vs-virtualenv-commands)

## 4.How to active conda in zsh?

  step 1: find the ".zshrc" file, and then vim it.

  step 2: export PATH=$HOME/miniconda3/bin:$PATH

  step 3: source .zshrc

  step 4: input conda --version in terminal,it will return the version if it works.

  Warning:In step 2,the path need to be the positon of miniconda3/miniconda/anaconda/anaconda3 or any other directory..
	  this path could be different each other. By default,the directory is in the $HOME.

## 5.How to manage packages in conda (including packages installed by pip and conda)
  
  Imaging a situation:your project requires an old package that is out-dated of conda, so you need to install the old package by pip.But after 'pip install <package-name>' in NEW conda environment,you 
                      input 'conda list' and expect to see if the package is installed. HOW A PITY...you didn't see any packages in your requirements.txt installed in NEW conda environment.
                      But when you switch the conda environment into 'base', you input 'conda list' again, you will see the list of packages in the terminal.what's going wrong? maybe you are confused.
                      So,HOW to install these old packages by pip in NEW conda environment? (you wanna see these packages after 'conda list' in the NEW conda environment)
                      Use: /anaconda/envs/venv_name/bin/pip install package_name
                      the path above may be different each other, the anaconda could be anaconda3/miniconda/miniconda3, the venv_name depends on your NEW conda environment name. By the way,there may be 
                      more pre-path depend where you install your anaconda/anaconda3/miniconda/miniconda3 
                      reference:[this help](https://www.puzzlr.org/install-packages-pip-conda-environment/)

