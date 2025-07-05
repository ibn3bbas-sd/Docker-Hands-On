FROM ubuntu:22.04

RUN apt-get update && apt-get install -y python3 python3-pip
RUN pip3 install flask

COPY app.py /opt/

ENV FLASK_APP=/opt/app.py
ENTRYPOINT ["flask", "run", "--host=0.0.0.0", "--port=8080"]