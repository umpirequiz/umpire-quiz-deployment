To deploy everything, first make sure you have no removed local docker images and containers, AND you have built and pushed the latest images. Then run:
```console
docker compose --env-file .\compose.env up
```

To log into the proxy manager, go to http://quiz.bramjanssens.local:81 with:
- s.a.janssens@gmail.com
- brambram