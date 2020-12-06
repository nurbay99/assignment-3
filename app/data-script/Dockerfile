FROM alpine

WORKDIR /opt

RUN apk update

RUN apk add mysql mysql-client

COPY import.sh /opt/
COPY mydatabase.sql /opt/
RUN chmod +x import.sh
CMD ./import.sh

