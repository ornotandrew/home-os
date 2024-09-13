# Home-OS

## UniFi

Instructions are on the [linuxserver repo](https://github.com/linuxserver/docker-unifi-network-application).

Specifically, see the "Device Adoption" section. The IP of the host needs to be set in the UniFi settings.

Note that the docker-compose definition expects some env vars - use `.env.template`.

### MongoDB

This is a dependency for UniFi. Grab the raspberrypi-compatible docker image from [here](https://github.com/themattman/mongodb-raspberrypi-docker).

When starting Mongo for the first time, uncomment the `init-mongo.js` volume to provision the unifi user.
