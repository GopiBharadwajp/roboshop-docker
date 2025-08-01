FROM python:3.9
EXPOSE 8080
WORKDIR /opt/server
COPY requirments.txt .
COPY *.py .
COPY payment.ini .
RUN pip3 install --no-cache-dir --prefix=/install -r requirements.txt
CMD ["uwsgi", "--ini", "payment.ini"]