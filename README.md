# neoloadTest

## Simple infrastructure 1 Controller + 1 LG
docker-compose -f nlweb-infra.yml up
docker-compose -f nlweb-infra.yml down

## Scale infrastructure
docker-compose -f nlweb-infra-scale.yml up --scale nlw-lg=2 --remove-orphans
docker-compose -f nlweb-infra-scale.yml down --scale nlw-lg=2 --remove-orphans