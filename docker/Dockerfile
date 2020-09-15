FROM continuumio/miniconda3

RUN conda update -n base conda
RUN conda install nb_conda_kernels
RUN git clone https://github.com/ccivit/DeViSE-zero-shot-classification/

WORKDIR /DeViSE-zero-shot-classification
RUN conda env create -f env.yml
RUN ipython kernel install --user --name=DeViSE_env
RUN source activate DeViSE_env
