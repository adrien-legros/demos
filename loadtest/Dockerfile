FROM registry.access.redhat.com/ubi8/ubi:8.0

COPY . /app
RUN dnf install -y python3 && pip3 install -r /app/requirements.txt && chmod -R a+rwx /app

EXPOSE 8080

CMD python3 /app/app.py
USER 1001
