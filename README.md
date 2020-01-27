# Let's Encrypt Installation

Runs Docker containers for Let's Encrypt and DuckDNS.

## Prerequisites

- Git
- Docker macvlan network named `local`

## Run with Docker Compose

1. Download the repository

   ```sh
    git clone https://github.com/devopsleigh/letsencrypt.git
    cd letsencrypt
    nano .env
    ```

2. Change secrets appropriately

   ```sh
   TZ=Country/City
   DUCKDNS_URL=yourdns.duckdns.org
   DUCKDNS_TOKEN=guid
   EMAIL=user@domain.com
   SUBDOMAINS=yourdns
   ```

3. Run the containers

   ```sh
   sudo docker-compose up -d --force-recreate
   ```
