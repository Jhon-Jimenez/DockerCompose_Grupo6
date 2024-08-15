FROM python:3.9-slim
WORKDIR /app_web
COPY . /app_web
RUN pip install -r requirements.txt
EXPOSE 8000
CMD python ./app_web.py