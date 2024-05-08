# netbox-docker

## Build Docker image
```
docker compose build --no-cache
```

## Bring up NetBox
```
docker compose up
```

## Set admin password
```
docker compose exec netbox /opt/netbox/netbox/manage.py createsuperuser
```

Browse to http://127.0.0.1:8080 and login with admin credentials set above.

## Bring down NetBox and remove data
```
docker compose down -v
```
