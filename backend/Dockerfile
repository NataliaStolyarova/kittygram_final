FROM python:3.9-slim

WORKDIR /app/requirements/

COPY requirements.txt .
COPY requirements.lint.txt .

RUN pip install -r requirements.txt --no-cache-dir
RUN pip install -r requirements.lint.txt --no-cache-dir

WORKDIR /app

COPY . .

ENTRYPOINT [ "sh", "docker-entrypoint.sh" ]
