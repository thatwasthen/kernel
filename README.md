In OSX, to create a named Jupyter kernel, use the following command:

env=$(basename `echo $CONDA_PREFIX`)
python -m ipykernel install --user --name "$env" --display-name "Python [conda env:"$env"]"
To read the list of all kernels created:

jupyter kernelspec list

and to delete an existing kernel:

jupyter kernelspec uninstall KERNELNAME
