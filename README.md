# Homelab

General informations about my homelab/home server.

## Table of contents

- [Apps](apps). List of the apps on my server.

## Hardware

| Component | Product                   |
| --------- | ------------------------- |
| OS        | Proxmox                   |
| CPU       | Intel® Core™ i5-12600K    |
| MOBO      | GIGABYTE B760 Gaming X AX |
| RAM       | 32GB DDR5 6000MHz CL30    |
| Storage   | 2x Seagate IronWolf 8To   |

## Architecture

```mermaid
architecture-beta
    group api(cloud)[API]

    service db(database)[Database] in api
    service disk1(disk)[Storage] in api
    service disk2(disk)[Storage] in api
    service server(server)[Server] in api

    db:L -- R:server
    disk1:T -- B:server
    disk2:T -- B:db
```
