FROM python:3.9.1

RUN apt-get install wget
RUN pip install pandas psycopg2 sqlalchemy
RUN mkdir -p /app/downloaded

WORKDIR /app
COPY ingest_data.py ingest_data.py

ENTRYPOINT [ "python" , "ingest_data.py"]
