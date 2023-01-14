FROM python:3.8-alpine
ADD streaming_data_reader.py .
RUN apk update \
    && apk add --virtual build-deps gcc python3-dev musl-dev \
    && apk add --no-cache mariadb-dev
RUN pip3 install --upgrade pip
RUN pip3 install --upgrade setuptools
RUN pip3 install ez_setup kafka-python mysql mysql-connector
