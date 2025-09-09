FROM debian:12

RUN apt update -y
RUN apt install php-fpm -y

COPY www.conf etc/php/8.2/fpm/pool.d/.

# -F forces to run in foreground, on debian the cmd is named php-fpm8.2
CMD ["php-fpm8.2", "-F"]