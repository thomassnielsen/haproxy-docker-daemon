# HAProxy Docker Daemon
HAProxy running in Docker as a daemon under Supervisor

## Run

Example showing a haproxy running as an SSL proxy.

```
docker run -d --name haproxy -p "443:443" \
-v /path/to/haproxy.cfg:/usr/local/etc/haproxy.cfg \ thomassnielsen/haproxy-docker-daemon
```

Note: If you want to provide a certificate, the easiest way is to mount the whole directory instead of just the config file, and add the certificate to the directory.

## Build yourself
```
docker build -t haproxy-daemon .
```

```
docker run -d --name haproxy -v /path/to/haproxy.cfg:/usr/local/etc/haproxy/haproxy.cfg haproxy-daemon
```
