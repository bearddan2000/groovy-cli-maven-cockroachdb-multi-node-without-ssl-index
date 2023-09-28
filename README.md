# groovy-cli-maven-cockroachdb-multi-node-without-ssl-index

## Description
Creates a small database table
called `dog`. This table, `dog`, has been normalized to 3NF.
All output normally
seen in a terminal will be in `log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

A groovy maven build, that connects to 3 node cluster
cockroach database without ssl.

## Tech stack
- groovy
- maven
  - postgres drivers

## Docker stack
- cockroachdb/cockroach:v19.2.2
- maven:3-openjdk-17

## To run
`sudo ./install.sh -u`
- [Master node webui](http://localhost:8000)
- [Slave node 1 webui](http://localhost:8001)
- [Slave node 2 webui](http://localhost:8002)

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`

## Credit
[Cockroach setup](https://github.com/s0rg/cockroach-compose)
