FROM docker.io/jupyter/datascience-notebook:2023-09-04

USER root
# Generally, Dev Container Features assume that the non-root user (in this case jovyan)
# is in a group with the same name (in this case jovyan). So we must first make that so.
RUN groupadd jovyan \
    && usermod -g jovyan -a -G users jovyan

USER jovyan

RUN python3 -m pip install jupyterlab-quarto