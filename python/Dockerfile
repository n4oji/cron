FROM python:3.9.0b4-alpine3.12
COPY my_cron /bin/my_cron
COPY root /var/spool/cron/crontabs/root
RUN chmod +x /bin/my_cron
CMD crond -l 2 -f