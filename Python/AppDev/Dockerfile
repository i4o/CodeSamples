FROM ubuntu:latest

RUN apt-get update -y && apt-get install -y python3-pip python3-dev
RUN pip3 install -r requirements.txt

COPY ./requirements.txt /app/requirements.txt
WORKDIR /app
COPY ./app/ /app
RUN chmod -R 777 /app

ENTRYPOINT ["python3"]

CMD ["myApi_ub.py"]