# Windows install instructions for PyMC3


To use `pymc3_mc_2019.ipynb` you need a working `pymc3` installation, version 3.6 or greater. This involves a `theano` dependency. To get this to work reliably you need to create a `conda` environment for `theano` and `pymc3` to work together:

        conda install nb_conda
        conda create pymc3
        activate pymc3
        conda install pymc3 matplotlib ipykernel scikit-learn graphviz mkl-service m2w64-toolchain sphinx pygpu
        pip install pydataset
        pip install git+https://github.com/pymc-devs/pymc3


Then you should be able to launch the notebook, set the kernel (Kernel/Change Kernel) to `Python 3 [conda env:pymc3]` and everything should work fine.