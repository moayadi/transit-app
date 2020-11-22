FROM ubuntu:16.04
RUN apt-get update -y
RUN apt-get install -y python3-pip && pip3 install mysql-connector-python hvac Flask
COPY . /app
WORKDIR /app
# RUN pip3 install mysql-connector-python hvac Flask
ENTRYPOINT ["python3"]
CMD ["app.py"]