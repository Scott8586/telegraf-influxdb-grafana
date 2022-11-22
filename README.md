# telegraf-influxdb-grafana

A docker-compose setup for Telegraf, influxdb (version 2), and Grafana on Synology

This is derivative of [docker-compose-influxdb-v2-grafana](https://github.com/ansjin/docker-compose-influxdb-v2-grafana), so check there to get back to basics

# Installation

1. Copy example.env to .env
2. Create a 32 character hex key to use as a token (use included `keygen.sh` or someother way of your choosing)
3. Fill in other basics such as default bucket (I use short hostname), and organization (I use my personal root domain)
4. Fill in PUID and PGID from your Synology accout (use `id` to get these values), and Timezone information
5. Fill in basic usernames and passwords to your liking.
6. Start with `docker-compose up` watch for any problems, then ^C quit, and eventually restart with `docker-compose up -d`
