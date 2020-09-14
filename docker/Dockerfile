FROM evheniy/docker-data-science

RUN conda install nb_conda_kernels
RUN conda env create -f env.yml
RUN ipython kernel install --user --name=DeViSE_env
RUN source activate DeViSE_env
