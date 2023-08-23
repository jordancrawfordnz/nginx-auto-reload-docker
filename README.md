**This repo is archived.** It's not being maintained and may no longer work. I recommend looking into more native approaches to reload configuration or another tool which can support auto-reloading.

--- 

# NGINX Auto Reload

Based off the official NGINX container, this image starts a Cron job that automatically reloads the NGINX configuration every day.

## Why?
I use [docker-letsencrypt-manager](https://github.com/bringnow/docker-letsencrypt-manager) to automatically renew my LetsEncrypt certificates. I found that when my certificates renew, NGINX would continue to use the old certificates.

With this image, NGINX will swap to the new certificates automatically.
