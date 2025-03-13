# YoutubeDL-Material Configuration Guide

## Update URLs for `ytdl_mongodb_connection_string`
After running the container, you need to find ip addresses needed then update the configuration with the correct **Container IP addresses**.

### Steps to Get Assigned Docker IPs:
1. Start your container.
2. Open a terminal in **ZimaOS/CasaOS**.
3. Run the following command to fetch the IP addresses:
   ```sh
   docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress}}' mongo-db
