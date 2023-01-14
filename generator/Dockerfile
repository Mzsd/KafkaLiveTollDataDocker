FROM python:3.8-alpine
ADD toll_traffic_generator.py .
RUN apk update \
    && apk add --virtual build-deps gcc python3-dev musl-dev
RUN pip3 install --upgrade pip
RUN pip3 install --upgrade setuptools
RUN pip install ez_setup kafka-python