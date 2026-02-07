# Personal APT Repository

Public Debian/Raspberry Pi OS APT repository.

## Add repository

```bash
curl -fsSL https://hoefling.io/apt/keys/repo-public.gpg \
  | sudo tee /usr/share/keyrings/hoefling-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/hoefling-archive-keyring.gpg] https://hoefling.io/apt stable main" \
  | sudo tee /etc/apt/sources.list.d/hoefling-private.list
```

```bash
sudo apt update
```

## Install packages

```bash
sudo apt install python3-aiogram
```

## Supported architectures

- arm64 (Raspberry Pi 5)
- amd64 (local testing)
