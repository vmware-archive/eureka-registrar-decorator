# Eureka Registrar Decorator

This is a [decorator](https://github.com/cf-platform-eng/meta-buildpack/blob/master/README.md#decorators) buildpack
for Cloud Foundry that provides integration with the Spring Cloud Eureka server *for any programming
language* supported by the platform, and requiring *zero application code changes*.

When this decorator (and the [meta-buildpack](https://github.com/cf-platform-eng/meta-buildpack))
is present in your Cloud Foundry deployment, all you will have to do to register all instances of your
application with the Eureka discovery server is bind the application to your Spring Cloud
Eureka Servive instance. Instances will then automatically be registered and continue to send heartbeats
as long as the application container is alive.


