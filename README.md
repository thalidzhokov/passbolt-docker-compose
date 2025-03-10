# passbolt-docker-compose
With SSL certificate by Letsencrypt

1. Create _.env_  ```cp .env.dist .env```
2. Create _docker-compose.override.yml_ ```cp docker-compose.override.yml.dist docker-compose.override.yml```
3. Create _traefik/traefik.yaml_ ```cp traefik/traefik.yaml.dist traefik/traefik.yaml```

4. Configure _.env_
5. Configure acme email and caServer AND log level in _traefik/traefik.yaml_

6. Run ```docker-compose up -d``` 
7. Create user ```docker exec passbolt su -m -c "bin/cake passbolt register_user -u your@email.com -f yourname -l surname -r admin" -s /bin/sh www-data``` and USE generated link to start registration

