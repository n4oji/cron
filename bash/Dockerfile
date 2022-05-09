FROM alpine:3.12
COPY my_cron /bin/my_cron
COPY root /var/spool/cron/crontabs/root
RUN chmod +x /bin/my_cron
# RUN chmod +x script.sh
RUN apk add --no-cache curl
CMD crond -l 2 -f