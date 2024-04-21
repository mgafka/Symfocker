# HOW-TO
1. Download https://github.com/mgafka/Symfocker/archive/refs/heads/master.zip and unpack in your project directory
2. Install mkcert https://github.com/FiloSottile/mkcert#installation
3. Go to your project
4. Go to `docker/nginx/certs` directory
5. Run `mkcert app_domain` where `app_domain` is the name of your app, e.g. `mkcert myapp.local`
6. Add app_domain to `/etc/hosts` file for Linux or `C:/Windows/System32/drivers/etc/hosts` for Windows
7. Change app domain and certs names in `docker/nginx/default.conf` file
8. Run `docker compose up -d`
