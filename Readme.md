### RabbitMQ on Docekr:
To run rabbitMQ on docker with management dashboard use:

``docker run --rm -it --hostname my-rabbit -p 15672:15672 -p 5672:5672 rabbitmq:3-management``


### Run Project
``python manage.py``

### Run Celery Workers (Use another terminal):
``celery -A main.celery worker --loglevel=info -Q universities,university``

