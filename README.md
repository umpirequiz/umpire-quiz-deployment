To deploy everything, run on a production server:
```console
docker compose --env-file .\compose.env up
```

## Local/test deployment

For local/test deployment, first change in `compose.yaml` > `services.reverse-proxy.volumes` to local volumes. Then:
```console
docker compose --env-file .\compose_local.env up
```

To import initial questions, use the importer service swagger ui (e.g. http://localhost:9082/openapi/ui/) to post the initial set from `importer_service/src/main/resources/sample-data.json`.
                
To create an admin user, use the user service swagger ui (http://localhost:9081/openapi/ui/) to post a user to the system with admin = true.  

To log into nginx proxy manager:
- http://localhost:81/
- s.a.janssens@gmail.com:firstnamefirstname

## Change log
- 0.8.0
  - added question counter 