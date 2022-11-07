FROM python:3.7-alpine

ENV PYTHONBUFFERED 1

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

RUN mkdir /djangoprojects
WORKDIR /djangoprojects
COPY ./djangoprojects /djangoprojects

RUN adduser -D user
USER user
