FROM mysql:5.7
COPY setup.sql /docker-entrypoint-initdb.d/
RUN chmod -R 775 /docker-entrypoint-initdb.d
RUN rm -rf /entrypoint.sh
COPY entrypoint.sh /
RUN chmod -R 775 entrypoint.sh

RUN apt-get update && apt-get install -y vim
