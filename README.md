# docker-webgrind
Docker container for running webgrind xdebug profiler analyzer

## Usage:

```bash
docker run -v /tmp:/tmp -p 8080:8080 madman/webgrind
```

## Configuration
You can configure following enviromental variables:

```bash
# Timezone
TIMEZONE="Europe/Kiev"

# This is the location where webgrind looks for the xdebug cachegrind files
XDEBUG_OUTPUT_DIR="/tmp"

# Here webgrind then stores the temp files after analyzing the results
WEBGRIND_STORAGE_DIR="/tmp/webgrind"

# Internal web server port number
PORT="8080"
```