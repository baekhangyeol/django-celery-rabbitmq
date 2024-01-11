FROM python:3.11-slim

COPY requirements.txt /
RUN pip install -r /requirements.txt

ADD . /api
WORKDIR /api

EXPOSE 8000

CMD python manage.py runserver 0.0.0.0:8000