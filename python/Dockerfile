FROM alpine:3.5

RUN apk add --update autoconf gcc g++ make bash git py2-pip python python-dev mariadb-dev libffi-dev

env APP_DIR /src/app

COPY requirements.txt ${APP_DIR}/requirements.txt

WORKDIR ${APP_DIR}

RUN pip install -r requirements.txt
