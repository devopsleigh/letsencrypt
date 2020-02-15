# Let's Encrypt Installation

Runs Docker containers for Let's Encrypt and DuckDNS.

## Prerequisites

- Git

## Run with Docker Compose

1. Download the repository

   ```sh
   git clone https://github.com/devopsleigh/letsencrypt.git
   cd letsencrypt
   nano .env
   ```

2. Change secrets appropriately

   ```yaml
   PATH_LETS_CONFIG=/path/to/share
   PATH_DUCK_CONFIG=/path/to/share
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
