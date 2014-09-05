# GeoServer build for the MTC2 SOA project

This project provides a way to consistently build a correctly-configured GeoServer WAR.

The source code for GeoServer and GeoTools are included with this project using git submodules.

## Instructions

To build a new `geoserver.war`, from the project's directory, issue the following command:

```Shell
mvn clean install -Papp-schema,wfs-notification,geoserver-sync -T1C -fae -DskipTests -pl war -am
```