FROM ubuntu:latest

# APT à jour
RUN apt-get update && apt-get upgrade -y

# Python & pip
RUN apt-get install -y python3 python3-pip

# (si nécessaire) lever la protection "externally managed"
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Flask via pip3 (exigé)
RUN pip3 install --no-cache-dir flask

# Préparer l'app
WORKDIR /app
COPY ./api.py /app/api.py

# Info de port (documentaire)
EXPOSE 5252

# Lancer Flask
CMD ["python3", "api.py"]







