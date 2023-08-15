
FROM nginx:1.9

# Copy the certs
COPY certs/ /etc/nginx/certs/

# Copy the proxy configuration
COPY proxy.conf /etc/nginx/conf.d/

# Copy the index.html file
COPY index.html /app/

# Change the permissions of all files, except for the SSL certificates
RUN chmod 777 /etc/nginx/*
RUN chmod 777 /app/index.html

EXPOSE 443
EXPOSE 80
