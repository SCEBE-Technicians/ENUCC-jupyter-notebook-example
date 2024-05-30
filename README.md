# jupyter-notebook-example

This repository serves as an example on how to execute a jupyter notebook on the ENUCC HPC cluster. There is a simple notebook called [NoisySine.ipynb](./NoisySine.ipynb). This notebook requires no user input and when run it produces an image of a scatter plot of a sine wave with some noise added, saved in the [figures](./figures) folder. In order to run the notebook, do the following:
```bash
$ git clone git@github.com:SCEBE-Technicians/jupyter-notebook-example.git
$ cd jupyter-notebook-example
$ conda env create -f env.yml
$ conda activate jupyter-example
$ srun jupyter execute NoisySine.ipynb
```

## Initialising conda

If you haven't run conda on ENUCC before then you'll have to run the following commands.

```bash
$ module load apps/anaconda3
$ conda init bash
```

Then you have to restart your shell, after which you will have access to conda.
