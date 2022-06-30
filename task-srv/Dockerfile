FROM hyperf/hyperf:8.0-alpine-v3.15-swoole-v4.8

WORKDIR /opt/www

COPY . /opt/www
RUN composer install --no-dev -o

EXPOSE 9506

ENTRYPOINT ["php", "/opt/www/bin/hyperf.php", "start"]
