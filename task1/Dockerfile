FROM ubuntu:latest

# Sistemi yeniləyirik
RUN apt-get update && apt-get upgrade -y

# Python3 və pip3 quraşdırırıq
RUN apt-get install -y python3 python3-pip

# "Externally managed" xətasını aradan qaldırırıq
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Flask-ı pip3 ilə quraşdırırıq
RUN pip3 install flask

# İşçi qovluğu və faylların kopyalanması
WORKDIR /app
COPY ./api.py /app/api.py

# Serveri işə salırıq
CMD ["python3", "/app/api.py"]
