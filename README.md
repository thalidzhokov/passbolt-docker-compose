# passbolt-docker-compose

1. Create _.env_  ```cp .env.dist .env```
2. Create _docker-compose.override.yml_ ```cp docker-compose.override.yml.dist docker-compose.override.yml```
3. Configure _.env_
4. Run ```docker-compose up -d``` 
5. Create user ```docker exec passbolt su -m -c "bin/cake passbolt register_user -u your@email.com -f yourname -l surname -r admin" -s /bin/sh www-data``` and USE link to start registration

