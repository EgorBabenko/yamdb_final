FROM python:3.7-slim

WORKDIR /api_yamdb


COPY requirements.txt /

RUN pip3 install -r /requirements.txt --no-cache-dir

COPY ./ .
COPY static/redoc.yaml static/redoc.yaml

CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ]
