FROM httpd:latest

RUN sed -i \
    -e '/#LoadModule deflate_module/s/^#//g' \
    -e '/#LoadModule proxy_module/s/^#//g' \
    -e '/#LoadModule proxy_fcgi_module/s/^#//g' \
    -e '/#Include conf\/extra\/httpd-vhosts.conf/s/^#//g' \
    /usr/local/apache2/conf/httpd.conf