FROM python:3.8

WORKDIR /crud

COPY ./crud /crud

RUN pip install -r /crud/requirements.txt

ENV SECRET_KEY hf9j!fg3k$50)jfd(!jk4dl45dkm!$fg1bc42cs7vb
ENV DEBUG 1

RUN python manage.py migrate

EXPOSE 8000

CMD gunicorn stocks_products.wsgi -b 0.0.0.0:8000
