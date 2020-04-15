# docker-compose-aprenda-quarkus
Docker Compose file including Postgres, Prometheus, Grafana and Keycloak images.

This file was created as support for the series of videos from Vinicius Ferraz.
https://www.youtube.com/watch?v=pBc0qSLaHO8&list=PLZzPRVfe8BbE6pVSv_9OMQPuoeQ71ZSMH

# Configuration
- Update the .env files with your desired user/password
- On Windows, add to hosts file: postgres, prometheus, grafana, keycloak
- Prometheus is using host.docker.internal:8080 to identify your Quarkus application on local host computer (outside docker)
