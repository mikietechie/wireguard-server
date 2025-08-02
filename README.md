# Wireguard VPN Server

A Wireguard VPN Server, for a Google Cloud VM!

## Getting Started

1. `touch .env`
2. `sudo docker compose -f "docker-compose.yml" up -d --build`

## Clients

Client configurations on the server are found by:

1. `sudo ls /wireguard/config`
2. `cat /wireguard/config/wg_confs/wg0.conf`

### Ubuntu Client

1. For a client called **peer1**. On server run `cat /wireguard/config/peer_peer1/peer_peer1.conf`.
2. On client paste into `sudo nano /etc/wireguard/peer_peer1.conf`
3. On client run using `wg-quick up peer_peer1`
