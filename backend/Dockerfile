FROM python:3.10-alpine AS builder
EXPOSE 8000
WORKDIR /app
COPY . /app/
RUN pip3 install -r requirements.txt --no-cache-dir
RUN chmod +x /app/entrypoint.sh
RUN /app/entrypoint.sh
ENTRYPOINT ["gunicorn"]
CMD ["backend.wsgi:application", "--bind", "0.0.0.0:8000"]
