# tailscale-web

## Getting started

Use the single line install script to install the latest version of tailscale-web.

```bash
curl -s https://raw.githubusercontent.com/luiseduardobrito/tailscale-web/main/install.sh | sudo bash

```

Or install manually following the steps below:


```bash
# Define your repository source
REPO="https://raw.githubusercontent.com/luiseduardobrito/tailscale-web/main";

# Prepare destination directory
mkdir -p "/etc/tailscale"

# Install shell init script
curl -o "/etc/tailscale/tailscale-web.sh" "$REPO/tailscale-web.sh";

# Install systemd service
curl -o "/etc/systemd/system/tailscale-web.service" "$REPO/tailscale-web.service";

# Reload systemd daemon
sudo systemctl daemon-reload;

# Start tailscale web
sudo systemctl enable --now tailscale-web.service;
```
