# HAProxy Docker Daemon
HAProxy running in Docker as a daemon under Supervisor

## Run
Instructions coming soon (not yet deployed on Docker Hub)

## Build yourself
```
docker build -t haproxy-daemon .
```

```
docker run -d --name haproxy -v /path/to/haproxy.cfg:/usr/local/etc/haproxy/haproxy.cfg haproxy-daemon
```
