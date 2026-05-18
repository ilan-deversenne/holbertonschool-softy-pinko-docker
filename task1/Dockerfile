FROM ubuntu:latest
WORKDIR /app

RUN apt-get update
RUN apt-get upgrade -y

COPY app/app.py .

RUN apt-get install python3 python3-pip -y
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip install flask

CMD ["python3", "app.py"]
