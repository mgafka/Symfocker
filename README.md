# HOW-TO
1. Go to your project and run `composer require `
2. Install mkcert https://github.com/FiloSottile/mkcert#installation
3. Go to `docker/nginx/certs` directory
4. Run `mkcert app_domain` where `app_domain` is the name of your app, e.g. `mkcert myapp.local`
5. Add app_domain to `/etc/hosts` file for Linux and `C:/Windows/System32/drivers/etc/hosts` for Windows
6. Change app domain and certs names in `docker/nginx/default.conf` file
7. Run `docker compose up -d`
