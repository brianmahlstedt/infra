Contains the docker composition for the nginx reverse proxy,
currently hosting southbaysupercontest.com and bmahlstedt.com
on a single digitalocean droplet.

You should only need to do the following once:
```bash
docker network create nginx-proxy
docker-compose up
```

The you can bring up any other containers running services
with `VIRTUAL_HOST`, etc.
