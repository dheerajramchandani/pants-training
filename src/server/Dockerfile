FROM python:3.7

RUN mkdir /app
WORKDIR /app

COPY ./src/server/ /app/
COPY ./3rdparty/requirements.txt /app/

RUN pip install -r requirements.txt

EXPOSE 50051

CMD ["python", "/app/greeter_server.py"]