# docker-compose-aprenda-quarkus
Docker Compose file including Postgres, Prometheus, Grafana and Keycloak images.

This file was created as support for the series of videos from Vinicius Ferraz.
https://www.youtube.com/watch?v=pBc0qSLaHO8&list=PLZzPRVfe8BbE6pVSv_9OMQPuoeQ71ZSMH

# Configuration
- Update the .env files with your desired user/password (default is admin / 123456)
- On Windows, add to hosts file: postgres, prometheus, grafana, keycloak
```
127.0.0.1 postgres
127.0.0.1 prometheus
127.0.0.1 grafana
127.0.0.1 keycloak
```
- You can start your environment by just running "docker-compose up"
- Prometheus contains a "aprenda-quarkus" job which is using "host.docker.internal:8080" to identify your Quarkus application on local host computer (localhost:8080) outside docker.
- The services are set to be accessible via: postgres:54320, jaeger:16686, prometheus:9090, grafana:3000 e keycloak:8180
