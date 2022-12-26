# diskover

## manual commands to run:

```shell
sysctl -w vm.max_map_count=262144
docker exec -it 33578dcda6eb python3 /app/diskover/diskover.py -i diskover-index0 /data
```

## notes:

needed to set `xpack.security.enabled=false` in order for diskover to connect to elasticsearch.  shouldn't be a problem given its entirely internal.

## TODO: 

- need ot be able to read files in /var/lib/docker/overlay2/