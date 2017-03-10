FROM nginx

ADD ./fastcgi-php.conf /etc/nginx/fastcgi-php.conf

ADD ./default.conf /etc/nginx/conf.d/default.conf

ADD ./fastcgi.conf /etc/nginx/fastcgi.conf

ADD ./nginx.conf /etc/nginx/nginx.conf

CMD service nginx restart
