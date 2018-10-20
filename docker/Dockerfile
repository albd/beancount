FROM python:3
COPY . /app
RUN pip install fava && \
	pip install /app/smart_importer
ENV PYTHONPATH "${PYTHONPATH}:/app"
WORKDIR /data
