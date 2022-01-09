# Using Virtual Environments with Jupyter Notebooks

Information on using python virtual environments with Jupyter Notebooks.

Source: <https://towardsdatascience.com/create-virtual-environment-using-virtualenv-and-add-it-to-jupyter-notebook-6e1bf4e03415>

If *virtualenv* is not installed, do so using: pip install virtualenv

1. Create a virtual environment using virtualenv. The following uses a virtualenv named "virt1jupyter".

> virtualenv virt1jupyter

2. Activate the virtual environment.

> source virt1jupyter/bin/activate

3. Install *ipykernal* using pip.

> pip install ipykernel

4. Add the virtual environment to Jupyter.

> python -m ipykernel install --user --name=virt1jupyter

It tells you where it installs the kernal that is the virtual environment. For me:

> /Users/dalemusser/Library/Jupyter/kernels/testjupyter1

In that directory is kernel.json that has the information Jupyter uses to know about this virtual environment kernel.

5. Open Jupyter Notebook and select *virt1jupyter* as the kernel. Go to *Kernel > Change kernel > virt1jupyter*



