# Docker Octopus Stack
Its ready to deploy and run into your Docker Swarm Cluster, there will be differend stack files you can run to get up and running with Docker Octopus.

## docker-full-master-stack.yml
Will spin a full stack up with all databases you need to run Docker Octopus in your system

``` bash
docker stack deploy -c docker-full-master-stack.yml octopus
```

## docker-master-stack.yml
Its will start what there need whit out eny databases running in Docker Swarm, its mean you need to setup RabbitMQ, MongoDB and InfluxDB at your self.

``` bash
docker stack deploy -c docker-master-stack.yml octopus
```

## docker-worker-stack.yml
Worker stack its the stack you need if you have more then one Docker Swarm Cluster and you want connect your to Docker Octopus system together.

``` bash
docker stack deploy -c docker-worker-stack.yml octopus
```