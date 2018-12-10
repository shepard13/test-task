FROM python:3.6

WORKDIR /opt/test-task

CMD cd /opt/test-task && \
    pip install -r requirements.txt && \
    pip install django-debug-toolbar && \
    pip install -r requirements/local.txt && \
    cp env.example .env && \
    python manage.py migrate && \
    python manage.py runserver