FROM python:3.7-slim

MAINTAINER sanjanadodley@gmail.com

RUN apt-get update -y && \
    apt-get install -y python-pip python-dev && \
    pip install --upgrade pip

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 80

ENTRYPOINT [ "python" ]

CMD [ "app.py" ]