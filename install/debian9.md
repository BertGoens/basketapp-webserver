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

- Start nginx: `sudo systemctl start nginx`  
- Restart nginx: `sudo systemctl restart nginx`
- Config check: `sudo nginx -t`
- Status check: `sudo systemctl status nginx`