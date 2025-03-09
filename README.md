# passbolt-docker-compose

1. Create _.env_  ```cp .env.dist .env```
2. Create _docker-compose.override.yml_ ```cp docker-compose.override.yml.dist docker-compose.override.yml```
3. Create _z-override.yaml_ ```cp z-override.yaml.dist traefik/conf/z-override.yaml```

4. Configure _.env_
5. Configure _traefik/config/z-override.yaml_

6. Run ```docker-compose up -d``` 
7. Create user ```docker exec passbolt su -m -c "bin/cake passbolt register_user -u your@email.com -f yourname -l surname -r admin" -s /bin/sh www-data``` and USE link to start registration

