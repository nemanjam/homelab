# Rathole client

- https://nitinja.in/tech/

- incoming traffic can be both 80 and 443
- cant resolve subdomain without decrypting https, Rathole must expose 80 and 443 exclusively on VPS
- can be done with VPS with two interfaces - IPs

- traefik on vps or local, matter of tunneling http or https
- git submodules for traefik-proxy repo
