# CUHackit_Demo


This repository contains the jupyter notebook and slides exported to PDF for reference. The code is there for you to tinker with and make the baseline network better. 


### Setting up a PyTorch Development Environment

For the purposes of this talk, we'll take advantage of the Palmetto Supercomputing Cluster. Convieniently, we have [JupyterHub](https://www.palmetto.clemson.edu) available to us for exploring jupyter notebooks. However, before we use that, we need to get our environment up and running. 

### Palmetto Setup:

Login to your palmetto login node and load the following modules:
```
1) anaconda/5.1.0 

2) cuda-toolkit/9.0.176   

3) cuDNN/9.0v7
```

You also want to create (or edit) a `.jhubrc` file and write these exact same lines to that file as well. Now our dev environment is ready to be created. Create a new conda environment like so:

```
conda create -n <my-name> python=3.5 
```
The `<my-name>` is to be replaced by a name of your choice. The name will be important in how you refer to your environment. Finally, we want to install `ipython` and then a **kernelspec** (this tells Jupyter to refer our anaconda environment). The kernel spec can now be installed like so:

```
python -m ipykernel install --user --name <my-name> --display-name <some-display-name> 
```

Once all of this is ready, we are all set to install `PyTorch` and then run our notebook. Simply clone this repo in your home directory and we're all set to go.

