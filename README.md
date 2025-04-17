# mars_allin_one
install in a node
docker-compose  operation:
1. docker-compose -f docker-compose.yml up -d
2. docker-compose -f docker-compose.yml stop

NOTE: ElasticSearch need run ./tools/setup_elasticsearch on host.

# build onos docker image
cd onos
ONOS_ROOT=$(pwd)

source $ONOS_ROOT/tools/dev/bash_profile
docker build -t onos:2.7 .
