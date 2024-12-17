FROM nginx:alpine

# Install nano, vim, and openssl in a single RUN command
RUN apk update && apk add --no-cache nano vim openssl

# Copy custom Nginx configuration files
COPY ./docker/nginx/nginx.conf /etc/nginx/nginx.conf
COPY ./docker/nginx/fastcgi-php.conf /etc/nginx/snippets/fastcgi-php.conf