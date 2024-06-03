# Rathole client

- https://nitinja.in/tech/

- incoming traffic can be both 80 and 443
- cant resolve subdomain without decrypting https, Rathole must expose 80 and 443 exclusively on VPS
- can be done with VPS with two interfaces - IPs

- traefik on vps or local, matter of tunneling http or https
- git submodules for traefik-proxy repo

```bash
# generate keys for noise protocol
docker run -it --rm rapiz1/rathole:v0.5.0 --genkey

# generate base64 secret
openssl rand -base64 32


# scp client config
scp ./rathole-client/rathole.client.toml username@192.168.1.120:~/homelab/traefik-proxy/core/rathole.client.toml

```
