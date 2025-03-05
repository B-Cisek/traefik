## docker compose service

```yml
   labels:
        - traefik.enable=true
        - traefik.http.routers.example-app.rule=Host(`test.online`)
        - traefik.http.routers.example-app.entrypoints=web
        - traefik.http.routers.example-app.tls=true
        - traefik.http.routers.example-app.tls.certresolver=cloudflare
    networks:
        - traefik
```
