# Basketapp

<img src="https://github.com/BertGoens/basketapp-backend/raw/master/media/logo.png" align="right" style="margin: 1.4em">

Main repo: [basketapp-backend](https://github.com/BertGoens/basketapp-backend)

## Why Nginx

Nginx has some advantageous features
- Easy to install
- Easy to configure
- Extremely fast at serving static files
- Works great as a reverse proxy
- Can do SSL signing

NodeJS is notoriously bad at serving static files and SSL. 
If we put Nginx in front of NodeJS we gain tremendous speed plus better security.

## Installing / Getting started
Download, install and start the service
```bash
# MacOS (Homebrew)
# Get homebrew at http://brew.sh
brew link pcre
brew install nginx
sudo nginx
# Ubuntu
sudo apt-get update
sudo apt-get install nginx
# Windows
# Download the latest nginx version at http://nginx.org/en/download.html
unzip nginx-1.3.13.zip
cd nginx-1.3.13
start nginx
```

## Editing the config
Modify `nginx.conf` and execute the following command to load the new config.

Make sure you didn't introduce any syntax errors by typing
```bash
# MacOs & Ubuntu
sudo nginx -t
# Windows 
nginx -t
```

## Restarting Nginx

```bash
# MacOS 
sudo nginx -s stop && sudo nginx
# Ubuntu
sudo service nginx restart
# Windows
nginx -s reload
```