#
# NOTE: THIS DOCKERFILE IS GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY.
#

FROM python:3.5-jessie

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY requirements.txt /usr/src/app/
RUN pip install --no-cache-dir  --upgrade tensorflow
RUN pip install --no-cache-dir -r requirements.txt

COPY ./tacotron /usr/src/app/tacotron

EXPOSE 9000