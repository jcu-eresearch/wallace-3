## Wallace Initiative

![CI build status](https://travis-ci.org/jcu-eresearch/wallace-3.svg?branch=master) 

The Wallace Initiative brings together experts in biodiversity (JCU, UEA), and climate change impacts and adaptation (UEA, JCU), with large datasets on the occurrence of biodiversity (GBIF) and the High Performance Computing Cluster and expertise at JCU to look at the potential impacts of climate change on global terrestrial biodiversity.  To date the project has generated 1 petabyte of data. If that petabyte was music it could play continuously for 2000 years, if it was video it would fill 223,000 DVDs or more than 13 years of HD video, if text it would fill 20 million four-drawer filing cabinets.  In other words it is a LOT of data on biodiversity and climate change.

### Setup

The Wallace web app is written in Python and depends on several external services in order to function:

* [`ElasticSearch`](https://github.com/jcu-eresearch/wallace-3/blob/master/docs/elasticsearch-install-log.md), originally installed on `wallace.hpc.jcu.edu.au`
* [`geoserver`](https://github.com/jcu-eresearch/wallace-3/blob/master/docs/geoserver-install-log.md) and corresponding [`nginx` config](https://github.com/jcu-eresearch/wallace-3/blob/master/docs/geoserver-nginx.conf), originally installed on `wallace-maps.hpc.jcu.edu.au`
* [Wallace web app](https://github.com/jcu-eresearch/wallace-3/blob/master/webapp/), originally installed on `wallace.hpc.jcu.edu.au`. Details on running the webapp are in its specific [`webapp/README.md`](https://github.com/jcu-eresearch/wallace-3/blob/master/webapp/README.md) and extra notes are described in the [docs](https://github.com/jcu-eresearch/wallace-3/blob/master/docs/wallace-install-log.md).
  * Wallace depends on specifically structured data and data files; the path configuration of which can be configured through [`webapp/production.ini`](https://github.com/jcu-eresearch/wallace-3/blob/master/webapp/production.ini).
  * An additional breakdown of the data flow is described by the [Collecting data diagram](https://github.com/jcu-eresearch/wallace-3/blob/master/docs/data-paths.md).

Details on how to set up and install these components can be found in at the links above. 

### Hardware specifications

The original server infrastructure called for two virtual machines to function, but it's feasible to only use one machine, adjusting the relevant paths and configuration to suit.  As a suggestion, the original infrastructure used the following as specifications:

* `wallace.hpc.jcu.edu.au`:
  * OS: RHEL 7
  * CPU: 2 vCPUs
  * RAM: 8GB
  * Storage: 100GB (OS), 10TB (data)
  * Network: Public access from the Internet; access to `wallace-maps.hpc.jcu.edu.au` required
* `wallace-maps.hpc.jcu.edu.au`: 
  * OS: RHEL 7
  * CPU: 2 vCPUs
  * RAM: 8GB
  * Storage: 100GB (OS and temp)
  * Network: Access to/from `wallace.hpc.jcu.edu.au` required
