# Download URL, write to UART or file

## Overview

This app implements an RPC service which allows to download a given URL
and write content to the UART or file. Example usage here fetches Mongoose OS
default firmware for ESP32 from mongoose-os.com and writes it to the UART 0:

Download to UART 0:

```
mos call Fetch '{"url": "http://mongoose-os.com/downloads/mos/version.json", "uart": 0}'
```

Download to a file:

```
mos call Fetch '{"url": "http://mongoose-os.com/downloads/mos/version.json", "file": "x.json"}'
```

