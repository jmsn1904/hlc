# Helpful Linux Commands

## Process Status (ps)

```bash
# Every process on the system:
ps aux
# Process tree:
ps axjf
ps auxf
```

## Socket Cat (socat)

```bash
# Proxy TCP Port
sudo socat TCP-LISTEN:66,fork,reuseaddr TCP:192.168.1.100:8080
```

### TODO List

(because I keep forgetting what I should be adding to this doc...)

- curl
- ffmpeg
- ip
- nmcli
- rg
- tar (!!!!)
