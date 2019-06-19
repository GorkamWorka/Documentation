## Priority R&D for cloud native tech and DevOps solution.

This is a compiled list of interesting tools and object, coming from CNCF Landscape maps. It is made as a reference desk of interesting technologies and opportunities for cloud tech and infrastructure development.  

Each Section represents a category of software, estimated Value of the section (personnal assesment) given in a 0-5 stars rating.  
Each list is ordinated by software predominance (again personnal assesment) and usability.  
Explaination and selection critera given on case by case basis. 
~ denote priority target (p.a. again)

### Cloud provider ***--

- [Digital Ocean](https://www.digitalocean.com): _already a provider, simple and efficient_
- [GKE](https://cloud.google.com/): _Major domain actor and the most advanced techno_
- [Azure](https://azure.microsoft.com/en-us/): _Microsoft, visual studio integration_

[ AWS is voluntarly ommited due to it being heavilly proprietary and non standard in lots of aspect. Basicly its either AWS or everything else on this page.]

### Automation & Configuration ****- 

- [Ansible](https://www.ansible.com): _Red Hat powered, Legendary level stability_
- ~[Chef](https://www.chef.io): _Most used by the community_

### Container Registry *****

- ~[Harbor](https://goharbor.io), independant docker image rregistry with a ton of added functionnality: _Well known and well loved by community, CNCF incubating project_
- ~[Portus](http://port.us.org), registry management and permissions dashboard: _SUSE powered, Very safe_
- [Azure Registry](https://azure.microsoft.com/en-us/services/container-registry), integrated Registry in Azure: _Azure_

### Security & Compliance *----

- [Open Policy Agent](https://www.openpolicyagent.org/): _Open source leader, CNCF Incubating project_

### Cloud-Native Storage *****

- ~[Rook](https://rook.io) shared and distributed storage and volume manager: _CNCF Incubating Project, loved by lots of influent people_
- [Minio](https://min.io) High performance Object storage: _most Stared, Excelent reputation_
- ~[etcd](https://github.com/etcd-io), key-values store : _CNCF incubating project, well supported_
- [Gluster](https://www.gluster.org/) quite the same as Rook : _Historic precursor, Red Hat powered_

### Container Runtime *----

- [rkt](https://github.com/rkt/rkt): _Most Stared, CNCF Incubating_
- [containerd](https://containerd.io): _CNCF Graduated, GKE default_

### Cloud-Native Network -----

(ususally handled by service mesh, hence low value)

- [Weave Net](https://www.weave.works/oss/net): _reliability, known name_

### Scheduling & Orchestration *****

- ~~[Kubernetes](https://kubernetes.io): _base of nearly anything else on this list, launched the cloud revolution_

### Coordination & Service Discovery *---- 

(ususally handled by service mesh, hence low value)

- [Netflix Eureka](https://github.com/Netflix/eureka): _Strong reliability, Netflix powered_ 
- [CoreDNS](https://coredns.io): _CNCF Graduated_

### Service Proxy **---

(ususally handled by service mesh, can be used separetly)

- [Traefik](https://traefik.io) edge routing, service routing: _Used in the docker stack, simple to use yet insanely powerfull_
- [Envoy](https://www.envoyproxy.io): _CNCF graduated, is used as a sidecart prowy by Istio_

### API Gateway **---

- [Kong](https://konghq.com): _most stared, stable_

### Service Mesh ****-

Service mesh are the basis for microservicing architecture and heavily automated self healing project.  
- ~~[Istio](https://istio.io): _Most active community, Powered by Google_ 
- [Netflix Zuul](https://github.com/Netflix/zuul): _known to be nearly unbreakable, Dev and Used by Netflix_
- [Linkerd](https://linkerd.io): _CNCF Graduated, historic actor_

### Database ****-

- ~[Redis](https://redis.io) Temporary and in memory storage, cache and multi layer database system : _flexibility, heavy usage and robustness, a stapple of the domain_
- [TiDB](https://pingcap.com/en), HTAP database MySQL compatible: _Quite popular, MySQL compatibility_
- [RethinkDB](https://www.rethinkdb.com), real time DB: _Linux foundation, popularity_
- [CockroachDB](https://www.cockroachlabs.com/), Cloud Native SQL: _popularity, compatible SQL_
- [Cassandra](https://cassandra.apache.org), large scale / big data database system: _apache Software Foundation powered, revered stability and quality_

### Streaming & Messaging **---

- [NATS](https://nats.io): _CNCF incubating, fast and efficient_
- [RabbitMQ](https://www.rabbitmq.com): _popularity_

### Application Definition & Image Build **---

- Docker Compose, **already used in the docker stack**
- ~~**[Helm](https://helm.sh), Kubernete manager**: _so much a stapple that most soft now provided helm install as primary install method_
- [OpenAPI](https://www.openapis.org), API Specifiaction and definition: _Very active community, heavilly supported_
- [kaniko](https://github.com/GoogleContainerTools/kaniko), Kubernete creating tool from docker image: _Widly used, Google powered_

### Continuous Integration & Delivery ****-

- [Gitlab](https://about.gitlab.com) Git management, project management, insanely good DevOps capability: _if you don't know why you need gitlab, they do_ 
- [Drone](http://try.drone.io): _Second most stared devOps Tool_
- [Concourse](https://concourse-ci.org/): _Complete and secure, Pivotal powered_

### Tools ****-

- ~~[Portainer](https://www.portainer.io) Container management visualisation and deplouement tool: _**already in use on dev stack** heap of cool features_

### Monitoring ***--

- [Netdata](https://my-netdata.io): _Realtime monitoring, hugely popular_
- ~[Grafana](https://grafana.com), **on dev stack** visualisation of monitoring and control data: _nice, personnal experience, share some code with Kibana (of ELK fame)_
- ~[Prométheus](https://prometheus.io), **on dev stack** monitoring data aggregation, enrichement and querying: _Hugely popular, safe and stable, personnal Experience_
- ~[Sentry](), **on dev stack** Error collection, monitoring and analysis: _quite popular, gitlab integration, personnal Experience_
- [Thanos](https://github.com/improbable-eng/thanos), High perf data persisting prometheus implementation: _well known, review globally extremly positive_
- [OpenMetrics](https://openmetrics.io) prometheus as a standar implementtation of prom: _CNCF Sandbox project, standardization_
- [Nagios](https://www.nagios.com/), network and host state monitor, service monitoring: _historical actor, personnal exp, paid version is insane (automated self healing and on event automation)_
- [Centreon](https://www.centreon.com/en), same function as Nagios; _More recent, viewend as safe_

### Logging **---

- [ELK](https://www.elastic.co) Elasticsearch, Logstash, Kibana. respectively Storage / query, log accretion and enrichment, visualiszation: _THE stapple solution for logging and visualisation, quite hard to master_
- [Fluentd](https://www.fluentd.org), logstash equivalent, log enrichement and agregation : _CNCF Graduated, reknown, quite popular_
- [OpenTracing](https://opentracing.io/), Tracing unification in Go : _CNCF incubating_
- [Jaeger](https://www.jaegertracing.io), Tracing unification : _CNCF incubating, well known_
