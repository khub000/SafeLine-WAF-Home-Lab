# Apache Configuration for DVWA

# Change Apache listening port
# File: /etc/apache2/ports.conf

Listen 8080

# Default Virtual Host
# File: /etc/apache2/sites-available/000-default.conf

<VirtualHost *:8080>
    ServerAdmin webmaster@localhost
    DocumentRoot /var/www/html/DVWA

    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>

# Restart Apache

sudo systemctl restart apache2
