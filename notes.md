New features

* Support downloading Docker images from private repositories in Amazon ECR. 
* Add the following parameters to customize the MQTT configuration on core devices:
    * maxInFlightPublishes – The maximum number of unacknowledged MQTT QoS 1 messages that can be in flight at the same time.
    * maxPublishRetry – The maximum number of times to retry a message that fails to publish.
* Add the fleetstatusservice configuration parameter to configure the interval at which the core device publishes device status to the AWS Cloud.

Bug fixes and improvements

* Fix an issue that caused shadow deployments to be duplicated when the nucleus restarts.
* Fix an issue that caused the nucleus to crash when it encountered a service load exception.
* Improve component dependency resolution to fail a deployment that includes a circular dependency.
* Fix an issue that prevented a public component from being redeployed if that component had been previously removed from the core device.
* Fix an issue that caused the HOME environment variable to be set to the /greengrass/v2/work directory for Lambda components or for components that run as root. The HOME variable is now correctly set to the home directory for the user that runs the component. 
* Additional minor fixes and improvements.
