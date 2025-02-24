
![Logo](https://user-images.githubusercontent.com/64506580/159311466-f720a877-6c76-403a-904d-134addbd6a86.png)

# Telegraf, InfluxDB, Grafana (TIG) Stack

Gain the ability to analyze and monitor telemetry data by deploying the TIG stack within minutes using [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/install/).

## ⚡️ Getting Started

Create an `.env` file from the `.env.sample` file, that will contain the environment variables that are used to setup and deploy the stack

```bash
├── telegraf/
├── .env         <---
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Customize the `telegraf.conf` file which will be mounted to the container as a persistent volume

```bash
├── telegraf/
│   ├── telegraf.conf <---
├── .env
├── docker-compose.yml
├── entrypoint.sh
└── ...
```

Start the services

```bash
docker-compose up -d
```

## Docker Images Used (Official & Verified)

[**Telegraf**](https://hub.docker.com/_/telegraf) / `1.24`

[**InfluxDB**](https://hub.docker.com/_/influxdb) / `2.5.1-alpine`

[**Grafana-OSS**](https://hub.docker.com/r/grafana/grafana-oss) / `9.2.3`
