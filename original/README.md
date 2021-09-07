This folder contains the notebooks with the examples used in the paper written with Bambi XXX. Here we provide instructions on how to set up an environment to reproduce the environment we originally used to obtain the results in the paper.

These instructions rely on [Anaconda](https://www.anaconda.com/). To begin, please install the [Anaconda individual edition that is compatible with your operating system](https://www.anaconda.com/products/individual).

This folder contains an `environment.yml` file that lists the packages needed to be able to run the notebooks. To install them, you first need to download the `environment.yml` file. Please note that if you have `git clone` this repository, the `environment.yml` file will have been downloaded too. Then, open a terminal (or Anaconda Prompt on Windows systems), go to the directory where the `environment.yml` is located and execute the following:

```bash
conda env create -f environment.yml
```

This will create an isolated conda environment called `bambi_joss` into which all of the listed packages and their requirements will be installed. You then have to activate the environment by executing the following in the same terminal window:

```bash
conda activate bambi_joss
```

Then, in the same terminal window, run either:

```bash
jupyter lab
```

or

```bash
jupyter notebook
```

This should open a jupyter notebook or lab tab in your default browser, where you will be able to start running all the code in the supplied notebooks.
