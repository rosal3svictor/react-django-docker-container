FROM python AS base

COPY requirements.txt /
RUN pip3 install --upgrade pip
RUN pip3 install -r /requirements.txt

FROM base AS dev-env
ENV APP=/server

WORKDIR $APP
VOLUME $APP