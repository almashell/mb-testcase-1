FROM python:3.7-slim

RUN mkdir /jupyter

RUN apt update
RUN apt-get install -y libglib2.0-0 libsm6 libxrender1 libxext6

RUN python3 -m pip install pandas matplotlib numpy notebook tqdm ipywidgets

RUN jupyter nbextension enable --py widgetsnbextension

WORKDIR /jupyter