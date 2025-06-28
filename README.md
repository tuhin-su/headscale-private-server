# BASIC COMMAND 
## Connect server with router and no dns
```bash
tailscale up --accept-routes --accept-dns=false --login-server=http://$IP
```
## Generate key for allow client to connect
```bash
hs preauthkeys create -e 24h -u $USER_NAME --authkey $KEY
```
## CREATE USER
```bash
hs users create $USER_NAME
```bash
alias hs="docker exec headscale headscale"
```
