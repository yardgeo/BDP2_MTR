FROM jupyter/datascience-notebook

RUN mkdir -p /usr/src/bdp2_mtr
COPY requirements.txt /usr/src/bdp2_mtr/
WORKDIR /usr/src/bdp2_mtr

RUN python3 -m pip install -r requirements.txt --no-cache-dir