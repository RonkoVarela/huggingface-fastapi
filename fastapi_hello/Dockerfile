FROM python:3.8

COPY ../requirements.txt /webapp/requirements.txt

WORKDIR /hello_world

RUN pip install -r requirements.txt

COPY hello_world/* /webapp

ENTRYPOINT [ "uvicorn" ]

CMD [ "--host", "0.0.0.0", "main:app" ]