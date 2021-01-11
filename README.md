# nginx-cheat-sheet
nginx cheat sheet with the most needed stuff.



# localhost

## create own domain
```bash
server {
    listen      0.0.0.0:80;
    server_name getstarted.com;

    location / {
        proxy_pass http://host.docker.internal:3000;
    }
}
```

/etc/hosts
```bash
127.0.0.1 getstarted.com
# ::1 = 127.0.0.1 in ipv6
::1 getstarted.com
```
