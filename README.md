# Personal APT Repository

Public Debian/Raspberry Pi OS APT repository.

## Add repository

```bash
echo "deb [trusted=yes] https://<username>.github.io/apt stable main" \
| sudo tee /etc/apt/sources.list.d/personal.list
```

```bash
sudo apt update
```

## Install packages

```bash
sudo apt install mytool
```

## Supported architectures

- arm64 (Raspberry Pi 5)
- amd64 (local testing)
