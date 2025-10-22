# Chromium with NoVNC

## Installation

- ### Manual
    ```sh
    docker run \
        --name chrome-novnc \
        -e PORT=8080 \
        -p 8080:8080 \
        -e VNC_PASS=CHANGE_IT \
        -d ghcr.io/niiwiicamo/chrome-novnc:latest
    ```

## Environment variables:
|VARIABLE         |DESCRIPTION              |DEFAULT VALUE  |
|----------------:|:------------------------|:-------------:|
|VNC_PASS         |VNC Password             |CHANGE_IT      |
|VNC_TITLE        |VNC Session Title        |Chromium       |
|VNC_SHARED       |VNC Shared Mode          |false          |
|VNC_RESOLUTION   |VNC Resolution           |1280x720       |
|SINGLETON_CLEANUP|cleans profile singleton |true           |
|USERAGENT        |Custom Useragent string  |""             |
