FROM nginx:latest

# copier les fichiers du site :
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# remplacer la config par défaut :
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# écoute sur ce port 
EXPOSE 9000
