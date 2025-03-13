# YoutubeDL-Material Configuration Guide

## Update URLs for `ytdl_mongodb_connection_string`
After running the container, you need to find the IP addresses and update the configuration with the correct **Container IP addresses**.

### Steps to Get Assigned Docker IPs:
1. Start your container.
2. Open a terminal in **ZimaOS/CasaOS**.
3. Run the following command to fetch the IP addresses:
   ```sh
   docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress}}' mongo-db


# Bonus Information

There are Chrome and Firefox extensions available that allow for a faster way to download videos, bypassing the need to open the GUI and manually copy/paste URLs. 

When the extension is activated while visiting a YouTube video, it will automatically fill in the URL. After installing the extension, you will need to configure it (right-click on the extension and select **Options**) with the YoutubeDL-Material GUI. 

Example: `http://192.168.1.***:8998`
---

**Project:** [YoutubeDL-Material](https://github.com/Tzahi12345/YoutubeDL-Material?tab=readme-ov-file)
