# esp-idf-container
[![Build ESP-IDF Tags](https://github.com/SergioGasquez/esp-idf-container/actions/workflows/build-tags.yml/badge.svg)](https://github.com/SergioGasquez/esp-rs-container/actions/workflows/build-tags.yml)

This repository contains Dockerfiles that create environments, using Debian
11.2, with all the necessary tools to develop applications for ESP boards with [Espressif IoT Development Framework](https://github.com/espressif/esp-idf)

In order to use it with Visual Studio Code Devcontainer or with Gitpod, please refer to
[esp-idf-devcontainer](https://github.com/SergioGasquez/esp-idf-devcontainer).

Using Git Hub actions, several tags for `linux/amd64` and for `linux/arm64`
platforms will be published into the
[sergiogasquez/esp-idf-env](https://hub.docker.com/r/sergiogasquez/esp-idf-env) image.
The tag naming follow the <idf_version>_<board> pattern, where:
- <idf_version> can be [v4.4](https://github.com/espressif/esp-idf/tree/v4.4) or [master](https://github.com/espressif/esp-idf/tree/master)
- <board> can be `esp32`, `esp32s2`, `esp32s3`, `esp32c3` or `all`