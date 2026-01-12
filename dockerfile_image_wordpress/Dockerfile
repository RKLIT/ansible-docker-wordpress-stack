#We use our basic image for this Dockerfile ansible-apache-php:latest
FROM ansible-apache-php:latest

#Install zip and unzip (It's for unzip WordPress)
RUN apt-get update && \
    apt-get install -y --no-install-recommends zip unzip && \
    rm -rf /var/lib/apt/lists/*

#Let's set environment variables
ENV WORDPRESS_VERSION=6.7.1

#Install and unzip WordPress
RUN curl -fsSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz" -o wordpress.tar.gz && \
    tar -xzf wordpress.tar.gz -C /var/www/html --strip-components=1 && \
    rm wordpress.tar.gz

#Rules for WordPress
RUN chown -R www-data:www-data /var/www/html && \
    chmod -R 755 /var/www/html/wp-content

#Port is 80
EXPOSE 80

# Start to Apache
CMD ["apache2-foreground"] 
