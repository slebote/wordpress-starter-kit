# WordPress starter kit

KIS (keep it simple) WordPress starter kit using official WordPress Docker image

## Index

1. Prerequisite
2. Installation

## 1. Prerequisite

* [Docker](https://docs.docker.com/) and [Docker compose](https://docs.docker.com/compose/)
* [CONTRIBUTING.md](CONTRIBUTING.md) guidelines and rules

## 2. Installation

```
cp .env-docker.sample .env
```

Adjust variables into `.env`

```
docker-compose up -d
sudo echo "wp-sk.local.fr" >> /etc/hosts
```

Consult [wp-sk.local.fr](https://wp-sk.local.fr) and accept self signed certificate issue
