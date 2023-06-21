FROM python:3.9-slim

WORKDIR /app

COPY . .

WORKDIR /app/requirements/

RUN pip install -r requirements.txt --no-cache-dir
RUN pip install -r requirements.lint.txt --no-cache-dir

ENTRYPOINT [ "sh", "docker-entrypoint.sh" ]
