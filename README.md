## 👋 Welcome to rustdesk 🚀

Open-source remote desktop software

## 📋 Description

Open-source remote desktop software

## 🚀 Services

- **server**: docker.io/rustdesk/rustdesk-server-pro:latest
- **relay**: docker.io/rustdesk/rustdesk-server-pro:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/rustdesk/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/rustdesk" ~/.local/srv/docker/rustdesk
cd ~/.local/srv/docker/rustdesk
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install rustdesk
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:21114

## 📂 Volumes

- `./rootfs/data/server` - Data storage
- `./rootfs/data/relay` - Data storage

## 🔍 Logging

```shell
docker compose logs -f server
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
