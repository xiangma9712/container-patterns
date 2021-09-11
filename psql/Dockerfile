FROM python:3.9

RUN apt-get update && apt-get install -y postgresql
RUN sed -i -e "s/peer/trust/g" `find /etc/postgresql -type f -name pg_hba.conf`

CMD bash