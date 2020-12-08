FROM mysql:latest

COPY ./products.csv /products.csv
COPY ./users.csv /users.csv

COPY ./migrate.sql /migrate.sql
COPY ./seed.sql /seed.sql
#COPY ./migrate_db.yaml /migrate_db.yaml
#COPY ./seed_db.yaml /seed_db.yaml

# COPY ./setup.sql /docker-entrypoint-initdb.d/setup.sql

ENTRYPOINT ["/entrypoint.sh"]
CMD ["mysqld", "--secure-file-priv=/"]
#CMD ["--secure-file-priv=/"]
