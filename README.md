# ARCHIVED REPO!!!!
repo was migrated here https://codeberg.org/dcraftbg/lake

# Lake

The new generation chat client infrastructure 

## Quickstart
Build System:
```
cc -o nob nob.c
```

Server:
```
./nob keygen run -- ./userA
./nob db-utils run -- -u ./userA.pub userA
./nob server run
```
Client:
```
./nob client run -- -key ./userA
```

**NOTE:**
Your client settings are saved in ~/.lake-tui:
```
~/.lake-tui/
    key.pub
    key.priv       
    server.conf    # hostname + port of server
```
For example:
~/.lake-tui/server.conf:
```toml
hostname = "localhost"
port = 8080
```
