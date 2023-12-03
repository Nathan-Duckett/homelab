# Homelab

Configuration files for my homelab setup.

Shortcut alias:
```bash
alias dlab="docker compose -f $HOME/dev/homelab/compose.yml --env-file $HOME/dev/homelab/.env"
```

Everything is built using docker compose V2 and included into the root docker compose file.

This makes use of [compose profiles](https://docs.docker.com/compose/profiles/).

To target a specific profile use the following commands:
```bash
dlab --profile smart_home up -d
dlab --profile smart_home logs -f
```