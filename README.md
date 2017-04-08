[View on GitHub](https://github.com/jordancrawfordnz/nginx-auto-reload)

[View on Docker Hub](https://hub.docker.com/r/jordancrawford/nginx-auto-reload/)

--- 

# NGINX Auto Reload

Based off the official NGINX container, this image starts a Cron job that automatically reloads the NGINX configuration every day.

## Why?
I use [docker-letsencrypt-manager](https://github.com/bringnow/docker-letsencrypt-manager) to automatically renew my LetsEncrypt certificates. I found that when my certificates renew, NGINX would continue to use the old certificates.

With this image, NGINX will swap to the new certificates automatically.
