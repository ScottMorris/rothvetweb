# rothvetweb
## Apache Configuration
### Ubuntu Server
1. Create a `rothvets` folder in `/var/www/` eg. `/var/www/rothvets`
2. Copy `000-rothvets.conf` in the config folder to the `/etc/apache2/sites-enabled/` folder.
3. Update `/etc/apache2/apache2.conf` with
```
<Directory /home/user/rothvetweb/>
        Options Indexes FollowSymLinks
        AllowOverride None
        Require all granted
</Directory>
```
4. Restart Apache, `sudo service apache2 restart`
