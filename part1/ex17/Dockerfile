FROM continuumio/miniconda3

RUN conda create -n env python=3.6
ENV PATH /opt/conda/envs/env/bin:$PATH

RUN conda update -n base -c defaults conda \
   && conda install -c anaconda nltk


