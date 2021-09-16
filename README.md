# alsa-utils

[![Build Status](https://github.com/squat/alsa-utils/workflows/CI/badge.svg)](https://github.com/squat/alsa-utils/actions?query=workflow%3ACI)
[![Docker Pulls](https://img.shields.io/docker/pulls/squat/alsa-utils?color=blue)](https://hub.docker.com/repository/docker/squat/alsa-utils)

This repository defines a multi-arch Docker image for [alsa-utils](https://github.com/alsa-project/alsa-utils).

## Usage

```bash
mkfifo fifo
docker run --rm --device=/dev/snd -v $(pwd):/var/lib/alsa-utils squat/alsa-utils arecord /var/lib/alsa-utils/fifo
```
