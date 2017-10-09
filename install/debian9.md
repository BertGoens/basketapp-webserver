# Debian 9 
## Installing / Getting started

```bash
sudo apt-get update
sudo apt-get install nginx
```

The configuration files can be found in
- /var/www/html
- /etc/nginx
- /etc/nginx/sites-available
- /etc/nginx/sites-enabled

## Nginx

- Start nginx: `sudo service nginx start`  
- Restart nginx: `sudo service nginx restart`
- Config check: `sudo nginx -t`