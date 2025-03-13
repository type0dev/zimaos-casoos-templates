# Archivist Configuration Guide

## Update URLs for `ES_URL` and `TA_HOS`
Before running the container, you need to update the configuration with the correct **Docker IP addresses**.

### Steps to Get Assigned Docker IPs:
1. Start your container.
2. Open a terminal in **ZimaOS/CasaOS**.
3. Run the following command to fetch the IP addresses:
   ```sh
   docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress}}' archivist-es archivist-redis
