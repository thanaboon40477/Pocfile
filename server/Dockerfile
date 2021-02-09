FROM python:3.8

COPY requirement.txt .
RUN pip install -r requirement.txt

COPY src/ /app
WORKDIR /app
CMD [ "uvcorn", "app:app" "--host" "0.0.0.0" "--port" "15400"]