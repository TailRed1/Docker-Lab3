FROM fedora:43

LABEL org.opencontainers.image.authors="Тимков Дмитро Віталійович"
LABEL org.opencontainers.image.version="1.0"

RUN dnf install -y httpd && dnf clean all

COPY index.html /var/www/html/index.html

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]