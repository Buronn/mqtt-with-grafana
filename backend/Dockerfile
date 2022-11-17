FROM python:3.7-alpine
RUN apk add --no-cache gcc musl-dev linux-headers
RUN pip install --upgrade pip
COPY requirements.txt /requirements.txt
RUN pip install -r /requirements.txt
COPY . /app
WORKDIR /app
CMD ["python","-u","app.py"]