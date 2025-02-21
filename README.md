application-dev.yml:

Environment: Development (Config-Dev)
  Application Name: Config-Dev
  Eureka Integration:
  Registers the service with Eureka.
  Configures the Config-Dev instance to prefer using the IP address for the service instance.
  Connects to the Eureka server running on localhost:8761.
  Purpose: This configuration is specifically for the development environment, where the application will register itself with Eureka as Config-Dev.
  application-prod.yml:

Environment: Production (Config-prod)
  Application Name: Config-prod
  Eureka Integration:
  Registers the service with Eureka.
  Configures the Config-prod instance to prefer using the IP address for the service instance.
  Connects to the Eureka server running on localhost:8761.
  Purpose: This configuration is specifically for the production environment. It registers the service under the name Config-prod in Eureka.
  application.yml:

Application Name: ConfigServer
  Eureka Integration:
  Configures the Config Server itself to register with Eureka as ConfigServer.
  Ensures that the Config Server instance uses the IP address for service registration.
  Connects to the Eureka server running on localhost:8761.
  Purpose: This configuration file defines the settings for the Config Server itself, which serves configuration properties to other microservices. It also registers the Config Server as a service in Eureka for discovery.
