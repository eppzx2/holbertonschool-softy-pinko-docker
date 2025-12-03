FROM ubuntu:latest
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED || true
RUN pip3 install flask
COPY api.py /api.py
EXPOSE 5252
CMD ["python3", "/api.py"]
