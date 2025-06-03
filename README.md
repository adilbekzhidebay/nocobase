Helm Chart for kubernetes

1) Pull repo
```
git pull https://github.com/adilbekzhidebay/nocobase.git
```
2) Create database and user (database owner)
3) Generate APP_KEY
```
openssl rand -base64 48
```
4) Create persistentVolume and persistentVolumeClaim
5) Set the environment variables NOCOBASE_PKG_USERNAME and NOCOBASE_PKG_PASSWORD (NocoBase Service Platform username and password) to automatically download commercial plugins during application installation or upgrade.
6) Create secrets for credentials such as database password, database user, app_key
7) Install or upgrade Helm Chart
```
helm upgrade --install nocobase nocobase/ -f nocobase.yml
```
