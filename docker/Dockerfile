FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential

# add requirements
COPY requirements.txt /app/requirements.txt

WORKDIR /app

# install requirements
RUN update-ca-certificates \
pip install -r requirements.txt

FROM base as app

WORKDIR /app

# add app
COPY ./ /app/

# run server
CMD python manage.py runserver

