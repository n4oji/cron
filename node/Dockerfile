FROM node:12.18.2-alpine3.9
COPY my_cron /bin/my_cron
COPY root /var/spool/cron/crontabs/root
RUN chmod +x /bin/my_cron
CMD crond -l 2 -f 