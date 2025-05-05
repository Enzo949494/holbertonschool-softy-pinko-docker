FROM nginx:latest

# Copy the front-end files into the directory expected by Nginx
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file (replaces default.conf)
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
