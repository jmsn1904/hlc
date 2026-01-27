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
- du
- ffmpeg
- fzf
- ip
- jq
- ln (because I always forget if source or destination comes first)
- nmap
- nmcli
- ping (just because there's some cool hidden flags imo)
- rclone or rsync ?
- rg
- tar (!!!!)
- tmux (sessions...)
