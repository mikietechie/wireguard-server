# Wireguard VPN Server

A Wireguard VPN Server, for a Google Cloud VM!

## Getting Started

1. `touch .env`
2. `sudo docker compose -f "docker-compose.yml" up -d --build`

## Clients

Client configurations are found in */wireguard/config*.

### Ubuntu Client

For a client called *peer1*. Copy the conf to a file in */etc/wireguard/peer1.conf*.
