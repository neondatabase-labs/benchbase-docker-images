# benchbase-docker-images
Generate a controlled version of benchbase docker images used for Neon benchmarking

## Purpose of this repository

[Benchbase](https://github.com/cmu-db/benchbase) (formerly OLTPBench) is a Multi-DBMS SQL Benchmarking Framework via JDBC [open sourced](https://db.cs.cmu.edu/projects/benchbase/) by Carnegie Mellon Database Group.

In Neon performance engineering we want to run benchmarks using benchbase and
- control the version of benchbase compatible with our setup
- build benchbase docker images for the architectures we use in our platform

This repository is used to build benchbase docker images for the architectures we use in our platform and make them publicly available on ghcr.io so that third parties can reproduce our published benchmark results.

The images are available here: https://github.com/neondatabase-labs/benchbase-docker-images/pkgs/container/benchbase-postgres and can be pulled with

```bash
# arm64
docker pull ghcr.io/neondatabase-labs/benchbase-postgres:latest-arm64
# amd64
docker pull ghcr.io/neondatabase-labs/benchbase-postgres:latest-amd64
```

