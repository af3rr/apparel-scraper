FROM python:3.7

WORKDIR /app

COPY . /app

RUN pip install -r requirements.txt

ENV PORT 8000
EXPOSE 8000

CMD ["gunicorn", "-b 0.0.0.0:8000", "app:app"]
