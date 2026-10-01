FROM postgres:15

COPY DDL_CalendarioLaboral.sql /docker-entrypoint-initdb.d/01-DDL_CalendarioLaboral.sql
COPY DML_CalendarioLaboral.sql /docker-entrypoint-initdb.d/02-DML_CalendarioLaboral.sql