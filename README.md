# tailscale-web

## Getting started

```bash
# Define your repository source
REPO="https://raw.githubusercontent.com/luiseduardobrito/tailscale-web/main";

# Install shell init script
curl -o "/etc/tailscale/tailscale-web.sh" "$REPO/tailscale-web.sh";

# Install systemd service
curl -o "/etc/systemd/system/tailscale-web.service" "$REPO/tailscale-web.service";
```
