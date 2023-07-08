# Shared network with Traefik

```bash
docker network create traefik_network
```

## Certificates

```bash
mkcert -install

mkcert -cert-file certs/local-cert.pem -key-file certs/local-key.pem "docker.localhost" "*.docker.localhost" "domain.local" "*.domain.local" "apps.local" "*.apps.local"
```
