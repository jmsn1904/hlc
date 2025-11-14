# Helpful Linux Commands

## Process status
```
### Every process on the system:
ps aux
### Process tree:
ps axjf
ps auxf
```
## Socat
```
### Proxy TCP Port
sudo socat TCP-LISTEN:66,fork,reuseaddr TCP:192.168.1.100:8080
```
