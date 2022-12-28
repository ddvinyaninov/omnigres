# Omnigres

Omnigres makes PostgreSQL a complete application platform. You can deploy a single database instance and it can host your entire application, scaling as needed.

* Running application logic **inside** or **next to** the database instance
* **Deployment** provisioning (**Git**, **Docker**, etc.)
* Database instance serves **HTTP**, **WebSocket** and other protocols
* In-memory and volatile on-disk **caching**
* Routine application building blocks (**authentication**, **authorization**, **payments**, etc.)
Database-modeled application logic via **reactive** queries
* Automagic remote **APIs** and **form** handling
* **Live** data updates

*This is a working-in-progress project at the moment and not ready for any kind of production use. If anything, it's at the prototyping stage.*

## Components

* [omni_containers](extensions/omni_containers/README.md)

## Try it out

To build and run Omnigres, you would currently need a recent C compiler, OpenSSL and cmake:

```shell
mkdir -p build && cd build
cmake ..
make psql_<COMPONENT_NAME> # for example, `psql_omni_containers`
```

Beware: this is currently more of a prototype and a lot is missing!