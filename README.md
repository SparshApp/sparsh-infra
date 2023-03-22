# sparsh-infra

## Architecture

![alt text](https://github.com/SparshApp/sparsh-infra/blob/main/docs/architecture.jpeg?raw=true)

## Setup

When you first set up Nginx, set the docker compose configuration in the other repositories, like sparsh-ui, to hide the exposed ports.

```bash
docker-compose up
```

## Ports

| Service | Port  |
| ------- | ----- |
| Nginx   | 80    |
| API     | 5001  |
| IOS     | 19006 |
| UI      | 3000  |  # Internal: use Nginx to access
| DB      | 5432  |  # Internal: use API to access
| ------- | ----- |
