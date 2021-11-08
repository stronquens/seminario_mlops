FROM jupyter/datascience-notebook:9b06df75e445

WORKDIR /home/jovyan/

COPY requirements.txt requirements.txt

COPY ejemplo.ipynb ejemplo.ipynb

# RUN apt-get update && apt-get install -y libpq-dev gcc

RUN pip install --upgrade pip

RUN pip install setuptools_rust

RUN pip install --ignore-installed PyYAML

RUN pip install -r requirements.txt

EXPOSE 8888
