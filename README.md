这个项目可以理解为针对互联网IT人打造的中文版awesome-go。已有的awesome-go项目， 汇总了很多go开源项目， 但存在的问题是收集太全了， 而且每个项目没有详细描述。

 本项目作为awesome-go的一个扩展，根据go语言中文社区提供的资料，还有互联网企业架构设计中的常见组件分类， 共精心挑选了154个开源项目（项目不限于在github开源的项目）， 分成以下17个大类。

 项目初衷是帮助到那些想学习和借鉴优秀golang开源项目， 和在互联网架构设计时期望快速寻找合适轮子的人。

ps: 以下项目**star数均大于100**，且会定期检查项目的url，剔除无效链接。 每个分类下的项目会按照**star数从高到低**进行排列。

[目录](#目录)

- [监控系统](#监控系统)
- [容器技术](#容器技术)
- [PaaS工具](#PaaS工具)
- [大数据](#大数据)
- [微服务](#微服务)
- [CI/CD](#CI/CD)
- [数据库技术](#数据库技术)
- [存储技术](#存储技术)
- [分布式系统](#分布式系统)
- [消息系统](#消息系统)
- [服务器管理](#服务器管理)
- [安全工具](#安全工具)
- [网络工具](#网络工具)
- [Web工具](#Web工具)
- [Web框架](#Web框架)
- [区块链技术](#区块链技术)
- [其它](#其它)

# 监控系统
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[grafana/grafana                      ](https://github.com/grafana/grafana)| Grafana 是一个用于监控指标分析和图表展示的工具， 后端支持 Graphite, InfluxDB & Prometheus & Open-falcon等， 它是一个流行的监控组件， 目前在各大中小型公司中广泛应用 |34113|
|[prometheus/prometheus                      ](https://github.com/prometheus/prometheus)| Prometheus 是一个开源的服务监控系统和时间序列数据库， 提供监控数据存储，展示，告警等功能 |29808|
|[bosun-monitor/bosun                      ](https://github.com/bosun-monitor/bosun)| 专业的跨平台开源系统监控项目，go语言编写，灵活的模板和表达式配合上各种collector可以监控任何应用或系统级的运行数据，比 zabbix更轻量级、更易入手和更适合定制。 |2961|
|[sourcegraph/checkup                      ](https://github.com/sourcegraph/checkup)| 一个分布式的无锁的站点健康状态检查工具。 支持检查http， tcp， dns等的状态 并可将结果保存在s3。 自带了一个美观的界面。 |2822|
|[influxdata/kapacitor                      ](https://github.com/influxdata/kapacitor)| Kapacitor 是一个开源框架，用来处理、监控和警告时间序列数据。      |1879|
|[rapidloop/rtop                      ](https://github.com/rapidloop/rtop)|rtop 是一个简单的无代理的远程服务器监控工具，基于 SSH 连接进行工作。无需在被监控的服务器上安装任何软件。rtop 直接通过 SSH 连接到待监控服务器，然后执行命令来收集监控数据。rtop 每几秒钟就自动更新监控数据，类似其他 *top 命令 |1845|
|[open-falcon/of-release                      ](https://github.com/open-falcon/of-release)| OpenFalcon是一款小米开源的监控系统。功能：数据采集免配置：agent自发现、支持Plugin、主动推送模式; 容量水平扩展：生产环境每秒50万次数据收集、告警、存储、绘图，可持续水平扩展。告警策略自发现：Web界面、支持策略模板、模板继承和覆盖、多种告警方式、支持回调动作。告警设置人性化：支持最大告警次数、告警级别设置、告警恢复通知、告警暂停、不同时段不同阈值、支持维护周期，支持告警合并。历史数据高效查询：秒级返回上百个指标一年的历史数据。Dashboard人性化：多维度的数据展示，用户自定义Dashboard等功能。架构设计高可用：整个系统无核心单点，易运维，易部署。 |1237|
|[rach/pome                      ](https://github.com/rach/pome)| Pome 是 Postgres Metrics 的意思。Pome 是一个 PostgreSQL 的指标仪表器，用来跟踪你的数据库的健康状况。 |1085|
|[gy-games/smartping                      ](https://github.com/gy-games/smartping)| SmartPing为一个各机器(点)间间互PING检测工具，支持互PING，单向PING，绘制拓扑及报警功能。 系统设计为无中心化原则，所有的数据均存储自身点中，默认数据循环保留1个月时间，由自身点的数据绘制 出PING包 的状态，由各其他点的数据绘制 进PING包 的状态，并API接口获取其他点数据绘制整体PING拓扑图，拓扑图中存在报警功能。 |856|
|[TalkingData/owl                      ](https://github.com/TalkingData/owl)| OWL是TalkingData公司推出的一款开源分布式监控系统, 演示环境http://54.223.127.87/ 登录账号密码demo/demo |758|
|[pinggg/pingd                      ](https://github.com/pinggg/pingd)| pingd 是世界上最简单的监控服务，使用 golang 编写。软件支持 IPv6，但是服务器不支持. pingd 允许同时 ping 上千个 IPs，在此期间还可以管理监控的主机。用户提供主机名或者 IP，还有用户邮箱地址，就可以使用 3 个生成 URLs 来开启，停止或者删除你的追踪。每当你的服务器停机或者后台在线都会发送通知，还包含控制 URLs。 |383|
|[cloudinsight/cloudinsight-agent                      ](https://github.com/cloudinsight/cloudinsight-agent)| 提供可视化监控的saas平台cloudinsight开源的一个监控客户端。 Cloudinsight 探针可以收集它所在操作系统的各种指标，然后发送到 Cloudinsight 后端服务 |357|
|[gravitational/satellite                      ](https://github.com/gravitational/satellite)| 用于监测kubernetes健康状态的一个工具／库。 其特点是：轻量级定期测试， 高可用性和弹性网络分区， 无单点故障， 以时间序列的格式存储监控数据。 |166|
|[kovetskiy/zabbixctl                      ](https://github.com/kovetskiy/zabbixctl)| Zabbixctl 是采用Zabbix服务API的命令行工具，它提供了有效的方式去查询和处理trigger 状态、主机最新数据和用户组。 |122|

# 容器技术
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[docker/docker                      ](https://github.com/docker/docker)| Docker 是一个开源的应用容器引擎，让开发者可以打包他们的应用以及依赖包到一个可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。容器是完全使用沙箱机制，相互之间不会有任何接口（类似 iPhone 的 app）。几乎没有性能开销,可以很容易地在机器和数据中心中运行。最重要的是,他们不依赖于任何语言、框架或包装系统。 |56684|
|[vmware/harbor                      ](https://github.com/vmware/harbor)| 容器应用的开发和运行离不开可靠的镜像管理。从安全和效率等方面考虑，部署在私有环境内的Registry是非常必要的。Project Harbor是由VMware公司中国团队为企业用户设计的Registry server开源项目，包括了权限管理(RBAC)、LDAP、审计、管理界面、自我注册、HA等企业必需的功能，同时针对中国用户的特点，设计镜像复制和中文支持等功能 |11230|
|[coreos/rkt                      ](https://github.com/coreos/rkt)| Rocket （也叫 rkt）是 CoreOS 推出的一款容器引擎，和 Docker 类似，帮助开发者打包应用和依赖包到可移植容器中，简化搭环境等部署工作。Rocket 和 Docker 不同的地方在于，Rocket 没有 Docker 那些为企业用户提供的“友好功能”，比如云服务加速工具、集群系统等。反过来说，Rocket 想做的，是一个更纯粹的业界标准。 |8914|
|[coreos/clair                      ](https://github.com/coreos/clair)| Clair 是一个容器漏洞分析服务。它提供一个能威胁容器漏洞的列表，并且在有新的容器漏洞发布出来后会发送通知给用户。 |6426|
|[shipyard/shipyard                      ](https://github.com/shipyard/shipyard)| Shipyard 是一个基于 Web 的 Docker 管理工具，支持多 host，可以把多个 Docker host 上的 containers 统一管理；可以查看 images，甚至 build images；并提供 RESTful API 等等。 Shipyard 要管理和控制 Docker host 的话需要先修改 Docker host 上的默认配置使其支持远程管理。 |6407|
|[zettio/weave                      ](https://github.com/zettio/weave)| Weave 创建一个虚拟网络并连接到部署在多个主机上的 Docker 容器。   |5798|
|[weaveworks/scope                      ](https://github.com/weaveworks/scope)| 一个docker&kubernetes的管理，监控可视化工具， 可以看到容器间的拓扑关系和tcp通信 |4206|
|[alibaba/pouch                      ](https://github.com/alibaba/pouch)| Pouch 是 Alibaba 公司开源的容器引擎技术，其主要功能包括基本的容器管理能力，安全稳定的强容器隔离能力，以及对应用无侵入性的富容器技术。 |4177|
|[docker/swarmkit                      ](https://github.com/docker/swarmkit)| SwarmKit 是Docker公司开源的Docker集群管理和容器编排工具，其主要功能包括节点发现、基于raft算法的一致性和任务调度等。 |2329|
|[emccode/rexray                      ](https://github.com/emccode/rexray)| REX-Ray 是一个 EMC {code} 团队领导的开源项目，为 Docker、Mesos 及其他容器运行环境提供持续的存储访问。其设计旨在囊括通用存储、虚拟化和云平台，提供高级的存储功能。 |1743|
|[docker/libnetwork                      ](https://github.com/docker/libnetwork)| Libnetwork 提供一个原生 Go 实现的容器连接，是容器的网络。libnetwork 的目标是定义一个健壮的容器网络模型（Container Network Model），提供一个一致的编程接口和应用程序的网络抽象。 |1612|
|[cloud66/habitus                      ](https://github.com/cloud66/habitus)| 一个快速实现docker build 流程的工具， 支持复杂的docker build流程，实现多个dockerfile的build流程，典型应用如将需要静态编译的程序，如go， java这类程序在一个docker build编译好之后，得到的二进制包用到后续的build流程 |1090|
|[vishvananda/wormhole                      ](https://github.com/vishvananda/wormhole)| WWormhole 是一个能识别命名空间的由 Socket 激活的隧道代理。可以让你安全的连接在不同物理机器上的 Docker 容器。可以用来完成一些有趣的功能，例如连接运行在容器本机的服务或者在连接后创建按需的服务。 |370|

# PaaS工具
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[kubernetes/kubernetes                      ](https://github.com/kubernetes/kubernetes)| Kubernetes 是来自 Google 云平台的开源容器集群管理系统。基于 Docker 构建一个容器的调度服务。该系统可以自动在一个容器集群中选择一个工作容器供使用。其核心概念是 Container Pod。 |64452|
|[rancher/rancher                      ](https://github.com/rancher/rancher)|Rancher2是基于Go编写的k8s管理平台，采用k8s in k8s的方式，极大的简化了k8s部署，并能同时管理多套k8s集群，操作和安全俱佳，是一款非常好的Devops工具|13922|
|[tsuru/tsuru                      ](https://github.com/tsuru/tsuru)| 在 Tsuru 的 PaaS 服务下，你可以选择自己的编程语言，选择使用 SQL 或者 NoSQL 数据库，memcache、redis、等等许多服务，甚至与你可以使用 Git 版本控制工具来上传你应用。 |3286|
|[laincloud/lain                      ](https://github.com/laincloud/lain)|   Lain 是一个基于 docker 的 PaaS 系统。其面向技术栈多样寻求高效运维方案的高速发展中的组织，devops 人力缺乏的 startup ，个人开发者。统一高效的开发工作流，降低应用运维复杂度；在 IaaS / 私有 IDC 裸机的基础上直接提供应用开发，集成，部署，运维的一揽子解决方案。      |449|
|[ooyala/atlantis                      ](https://github.com/ooyala/atlantis)| Atlantis 是一款基于 Docker，使用 Go 编写，为 HTTP 应用准备的开源 PaaS。Atlantis 可以在路由请求中轻松的构建和部署应用到容器。Atlantis 在 Ooyala 的新应用中得到了很广泛的应用。 |385|
|[weibocom/opendcp                      ](https://github.com/weibocom/opendcp)|   OpenDCP是一个基于Docker的云资源管理与调度平台，集镜像仓库、多云支持、服务编排、服务发现等功能与一身，支持服务池的扩缩容，其技术体系源于微博用于支持节假日及热点峰值流量的弹性调度DCP系统。OpenDCP允许利用公有云服务器搭建起适应互联网应用的IT基础设施，并且将运维的工作量降到最低。      |381|
|[mesos/cloudfoundry-mesos                      ](https://github.com/mesos/cloudfoundry-mesos)| Cloud Foundry-Mesos框架由华为与Mesosphere的工程师合作完成，能够为应用提供安全可靠的、可伸缩、可扩展的云端运行环境，并且应用能够 享用Cloud Foundry生态圈内各类丰富的服务资源。企业能够通过Cloud Foundry开发云应用，并通过Cloud Foundry-Mesos将应用部署到DCOS上，使应用能够与DCOS上安装的其他服务及应用框架共享资源，实现资源利用率最大化，能够大幅降低企业 数据中心运营成本。DCOS能够运行在虚拟和物理环境上，能够支持Linux（以及很快支持Windows），并可适用于私有云、公有云及混合云环境。 |107|

# 微服务
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[istio/istio                      ](https://github.com/istio/istio)| Istio是由Google、IBM和Lyft开源的微服务管理、保护和监控框架。使用istio可以很简单的创建具有负载均衡、服务间认证、监控等功能的服务网络，而不需要对服务的代码进行任何修改。 |22197|
|[go-kit/kit                      ](https://github.com/go-kit/kit)| Go-kit 是一个 Go 语言的分布式开发包，用于开发微服务。         |16516|
|[uber/jaeger                      ](https://github.com/uber/jaeger)| Jaeger是Uber的分布式跟踪系统 ，基于google dapper的原理构建， 以Cassandra作为存储层     |10479|
|[micro/micro                      ](https://github.com/micro/micro)| Micro是一个专注于简化分布式系统开发的微服务生态系统。可插拔的插件化设计，提供强大的可插拔的架构来保证基础组件可以被灵活替换。|7764|
|[eBay/fabio                      ](https://github.com/eBay/fabio)| fabio 是 ebay 团队用 golang 开发的一个快速、简单零配置能够让 consul 部署的应用快速支持 http(s) 的负载均衡路由器。这里有一篇中文文章http://dockone.io/article/1567介绍了如何用fabio＋consul实现服务发现，负载均衡，并阐述了原理， 最后还有demo程序 |6289|
|[goadesign/goa                      ](https://github.com/goadesign/goa)| Goa 是一款用 Go 用于构建微服务的框架，采用独特的设计优先的方法。     |3757|
|[NYTimes/gizmo                      ](https://github.com/NYTimes/gizmo)| 纽约时报开源的go微服务工具.提供如下特性:标准化配置和日志;可配置策略的状态监测端点;用于管理 pprof 端点和日志级别的配置;结构化日志，提供基本请求信息;端点的有用度量;优雅的停止服务; 定义期待和词汇的基本接口 |3076|
|[koding/kite                      ](https://github.com/koding/kite)| 一个基于go语言的微服务框架, Kite是Koding公司内部的一个框架, 该框架提供服务发现，多种认证功能，服务端通过RPC进行通信，同时还提供了websocket的js库，方便浏览器于服务器间进行通信。 |2709|
|[afex/hystrix-go                      ](https://github.com/afex/hystrix-go)| 用来隔离远程系统调用， 第三方库调用 ，服务调用， 提供熔断机制，避免雪崩效应的库， Hystrix的go 版本。 注Hystrixs是Netflix开源的一个java库 |2407|
|[fagongzi/gateway                      ](https://github.com/fagongzi/gateway)| Gateway是一个使用go实现的基于HTTP的API 网关。**特性** ：API 聚合 ; 流控;  熔断; 负载均衡; 健康检查;  监控;  消息路由;  后端管理WebUI .  **能做什么**：规划更友好的URL给调用者。聚合多个API的结果返回给API调用者，利于移动端，后端可以实现原子接口。保护后端API服务不会被突发异常流量压垮。提供熔断机制，使得后端API Server具备自我恢复能力。借助消息路由能力，实现灰度发布，AB测试。 |2364|
|[goodrain/rainbond                      ](https://github.com/goodrain/rainbond)| 云帮是一款以应用为中心的开源PaaS，深度整合Kubernetes的容器管理和Service Mesh微服务架构最佳实践，满足支撑业务高速发展所需的敏捷开发、高效运维和精益管理需求 |2195|
|[sourcegraph/appdash                      ](https://github.com/sourcegraph/appdash)| go版本的分布式应用跟踪系统， 基于google dapper的原理构建     |1622|
|[andot/hprose                      ](https://github.com/andot/hprose)| Hprose 是高性能远程对象服务引擎（High Performance Remote Object Service Engine）的缩写 —— 微服务首选引擎。它是一个先进的轻量级的跨语言跨平台面向对象的高性能远程动态通讯中间件。它不仅简单易用，而且功能强大。你只需要稍许的时间去学习，就能用它轻松构建跨语言跨平台的分布式应用系统了。 |609|

# CI/CD
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[drone/drone                      ](https://github.com/drone/drone)| Drone 是一个基于 Docker 的持续发布平台，使用 Go 语言开发    |20737|
|[caicloud/cyclone                      ](https://github.com/caicloud/cyclone)| Cyclone 是一个打造容器工作流的云原生持续集成持续发布平台，简单易用，使用 Go 语言开发，有详尽的中文文档 |877|

# 数据库技术
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[pingcap/tidb                      ](https://github.com/pingcap/tidb)| TiDB 是国内 PingCAP 团队开发的一个分布式 SQL 数据库。其灵感来自于 Google 的 F1, TiDB 支持包括传统 RDBMS 和 NoSQL 的特性。 |22947|
|[influxdata/influxdb                      ](https://github.com/influxdata/influxdb)| 一个可以水平扩展的时间序列数据库， 内建http api， 支持对数据打tag，灵活的查询策略和数据的实时查询，支持类sql语句进行查询 |18525|
|[cockroachdb/cockroach                      ](https://github.com/cockroachdb/cockroach)| CockroachDB (蟑螂数据库）是一个可伸缩的、支持地理位置处理、支持事务处理的数据存储系统。CockroachDB 提供两种不同的的事务特性，包括快照隔离（snapshot isolation，简称SI）和顺序的快照隔离（SSI）语义，后者是默认的隔离级别。 |17960|
|[google/cayley                      ](https://github.com/google/cayley)| Cayley 是 Google 的一个开源图(Graph)数据库，其灵感来自于 Freebase 和 Google 的 Knowledge Graph 背后的图数据库。 |13277|
|[dgraph-io/dgraph                      ](https://github.com/dgraph-io/dgraph)| dgraph 是可扩展的，分布式的，低延迟图形数据库。DGraph 的目标是提供 Google 生产水平的规模和吞吐量，在超过TB的结构数据里，未用户提供足够低延迟的实时查询。DGraph 支持 GraphQL 作为查询语言，响应 JSON。 |12759|
|[wandoulabs/codis                      ](https://github.com/wandoulabs/codis)| Codis 是一个分布式 Redis 解决方案, 对于上层的应用来说, 连接到 Codis Proxy 和连接原生的 Redis Server 没有明显的区别 (不支持的命令列表), 上层应用可以像使用单机的 Redis 一样使用, Codis 底层会处理请求的转发, 不停机的数据迁移等工作, 所有后边的一切事情, 对于前面的客户端来说是透明的, 可以简单的认为后边连接的是一个内存无限大的 Redis 服务. |10927|
|[youtube/vitess                      ](https://github.com/youtube/vitess)| outube出品的开源分布式MySQL工具集Vitess，自动分片存储MySQL数据表，将单个SQL查询改写为分布式发送到多个MySQL Server上，支持行缓存（比MySQL本身缓存效率高），支持复制容错，已用于Youtube生产环境 |9720|
|[sosedoff/pgweb                      ](https://github.com/sosedoff/pgweb)| gweb 是一个采用 Go 语言开发的基于 Web 的 PostgreSQL 管理系统。 |6325|
|[flike/kingshard                      ](https://github.com/flike/kingshard)| 一个高性能的mysql中间件， 支持读写分离， 数据分片， 安全审计等功能    |5070|
|[olivere/elastic                      ](https://github.com/olivere/elastic)| elastic是开源搜索引擎elasticsearch的golang客户端，API友好，支持绝大部分es的接口,支持的es版本全面，从1.x到最新的6.x全覆盖|4822|
|[siddontang/ledisdb                      ](https://github.com/siddontang/ledisdb)| ledisdb是一个参考ssdb，采用go实现，底层基于leveldb，类似redis的高性能nosql数据库，提供了kv，list，hash以及zset数据结构的支持。 |3246|
|[XiaoMi/Gaea                      ](https://github.com/XiaoMi/Gaea)|Gaea是小米商城/系统组研发的基于mysql协议的数据库中间件，目前在小米商城大陆和海外得到广泛使用。 |1408|
|[outbrain/orchestrator                      ](https://github.com/outbrain/orchestrator)| MySQL 复制拓扑可视化工具                          |787|
|[slicebit/qb                      ](https://github.com/slicebit/qb)| qb是用来让使更容易使用数据库的go语言的数据库工具包。它受Python最喜欢的ORM SQLAlchemy的启发，既是一个ORM，也是一个查询生成器。它在表达api和查询构建东西的情形下是相当模块化的。 |524|
|[hidu/mysql-schema-sync                      ](https://github.com/hidu/mysql-schema-sync)| mysql-schema-sync 是一款使用go开发的、跨平台的、绿色无依赖的 MySQL 表结构自动同步工具。用于将线上(其他环境)数据库结构变化同步到测试（本地）环境! |418|
|[chasex/redis-go-cluster                      ](https://github.com/chasex/redis-go-cluster)| redis-go-cluster 是基于 Redigo 实现的 Golang Redis 客户端。redis-go-cluster 可以在本地缓存 slot 信息，并且当集群修改的时候会自动更新。此客户端管理每个节点连接池，使用 goroutine 来尽可能的并发执行，达到了高效，低延迟。 |375|
|[mediocregopher/radix                      ](https://github.com/mediocregopher/radix)| radix是redis官方推荐的客户端之一，相比于redigo,radix.v2特点是轻量、接口实现优雅、API友好|327|
|[goshawkdb/server                      ](https://github.com/goshawkdb/server)| GoshawkDB 是一个采用 Go 语言开发支持多平台的分布式的对象存储服务，支持事务以及容错。GoshawkDB 的事务控制是在客户端完成的。GoshawkDB 服务器端使用 AGPL 许可，而 Go 语言客户端使用 Apache 许可证 |204|
|[degdb/degdb                      ](https://github.com/degdb/degdb)| DegDB 是分布式的经济图数据库。                       |201|

# 存储技术
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[ipfs/go-ipfs                      ](https://github.com/ipfs/go-ipfs)| IPFS 是分布式文件系统，寻求连接所有计算机设备的相同文件系统。在某些方面，这很类似于原始的 Web 目标，但是 IPFS 最终会更像单个比特流群交换的 git 对象。IPFS ＝ InterPlanetary File System |9425|
|[chrislusf/seaweedfs                      ](https://github.com/chrislusf/seaweedfs)| SeaweedFS 是简单，高伸缩性的分布式文件系统，包含两部分：存储数十亿的文件；快速为文件服务。SeaweedFS 作为支持全 POSIX 文件系统语义替代，Seaweed-FS 选择仅实现 key-file 的映射，类似 "NoSQL"，也可以说是 "NoFS"。 |9348|
|[spf13/afero                      ](https://github.com/spf13/afero)| Afero 是一个文件系统框架，提供一个简单、统一和通用的 API 和任何文件系统进行交互，作为抽象层还提供了界面、类型和方法。Afero 的界面十分简洁，设计简单，舍弃了不必要的构造函数和初始化方法。Afero 作为一个库还提供了一组可交互操作的后台文件系统，这样在与 Afero 协作时，还可以保留 os 和 ioutil 软件包的功能和好处。 |2631|
|[coreos/torus                      ](https://github.com/coreos/torus)| Torus是一种针对容器集群量身打造的存储系统，可以为通过Kubernetes编排和管理的容器集群提供可靠可扩展的存储。这是继etcd、rkt、flannel，以及CoreOS Linux之后CoreOS发布的另一个开源产品。 |1800|
|[emccode/rexray                      ](https://github.com/emccode/rexray)| REX-Ray 是一个 EMC {code} 团队领导的开源项目，为 Docker、Mesos 及其他容器运行环境提供持续的存储访问。其设计旨在囊括通用存储、虚拟化和云平台，提供高级的存储功能。 |1743|
|[Terry-Mao/bfs                      ](https://github.com/Terry-Mao/bfs)| bfs 是使用 Go 编写的分布式文件系统（小文件存储）。            |1133|
|[gostor/gotgt                      ](https://github.com/gostor/gotgt)| Gotgt 是使用 Go 编写的高性能、可扩展的 iSCSI target 服务。    |161|

# 分布式系统
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[chrislusf/seaweedfs                      ](https://github.com/chrislusf/seaweedfs)| SeaweedFS 是简单，高伸缩性的分布式文件系统，包含两部分：存储数十亿的文件；快速为文件服务。SeaweedFS 作为支持全 POSIX 文件系统语义替代，Seaweed-FS 选择仅实现 key-file 的映射，类似 "NoSQL"，也可以说是 "NoFS"。 |9348|
|[kelseyhightower/confd                      ](https://github.com/kelseyhightower/confd)| Confd是一个轻量级的配置管理工具。通过查询Etcd，结合配置模板引擎，保持本地配置最新，同时具备定期探测机制，配置变更自动reload。 |6887|
|[hashicorp/nomad                      ](https://github.com/hashicorp/nomad)| Nomad 是一个集群管理器和调度器，专为微服务和批量处理工作流设计。Nomad 是分布式，高可用，可扩展到跨数据中心和区域的数千个节点。 |5944|
|[chrislusf/glow                      ](https://github.com/chrislusf/glow)| Glow 是使用 Go 编写的易用分布式计算系统，是 Hadoop Map Reduce，Spark，Flint，Samza 等等的替代品。Glow 的目标是提供一个库，可以在并行线程或者分布式集群机器中进行更简单计算。 |2760|
|[chrislusf/gleam                      ](https://github.com/chrislusf/gleam)| 此处是一个通过Go和LuaJIT编写的快速和可扩展的分布式map/reduce系统，很好的将Go的高并发性与Luajit高性能相结合，可独立运行或用于分布式计算。 |2420|
|[purpleidea/mgmt                      ](https://github.com/purpleidea/mgmt)| mgmt 是一个分布式的，事件驱动的配置管理工具。该工具支持并行执行，其 librarification 作为新的及已存在的软件的基础管理工具。 |2197|
|[youtube/doorman                      ](https://github.com/youtube/doorman)| Doorman 是一个客户端速率限制的解决方案，客户端与共享资源进行通讯，包括数据库、gRPC 服务、RESTful API 等等可使用 Doorman 来限制对资源的调用。Doorman 使用 Go 语言开发，使用 gRPC 的通讯协议。其高可用特性需要一个分布式的锁管理器，当前支持 etcd，也可使用 Zookeeper 替代。 |1521|
|[nanopack/yoke                      ](https://github.com/nanopack/yoke)| Yoke 是 Postgres 的高可用集群，具有自动切换和自动集群恢复。Postgres冗余/自动故障转移解决方案，提供一个高可用PostgreSQL集群的简单管理。 |1372|
|[huichen/zerg                      ](https://github.com/huichen/zerg)| 基于docker的分布式爬虫服务                         |464|
|[silenceper/dcmp                      ](https://github.com/silenceper/dcmp)| DCMP是分布式配置管理平台。提供了一个etcd的管理界面，可通过界面修改配置信息，借助confd可实现配置文件的同步。 |193|

# 消息系统
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[bitly/nsq                      ](https://github.com/bitly/nsq)| NSQ 是无中心设计、节点自动注册和发现的开源消息系统。可作为内部通讯框架的基础，易于配置和发布。 |17388|
|[RichardKnop/machinery                      ](https://github.com/RichardKnop/machinery)| Machinery 是一个 Go 语言的异步任务队列和作业队列，基于分布式消息传递。类似 Python 的 Celery 框架。 |3902|
|[blackbeans/kiteq                      ](https://github.com/blackbeans/kiteq)| KiteQ 是一个基于 go + protobuff 实现的多种持久化方案的 mq 框架（消息队列）。 |742|

# 服务器管理
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[gravitational/teleport                      ](https://github.com/gravitational/teleport)| teleport 是 初创公司Gravitational 的一款基于ssh和https的远程管理linux 集群服务器的工具， 其特点是支持双重校验登陆；操作记录回放；session共享，便于协作排障；自动发现集群的服务器和容器 |7928|
|[square/sharkey                      ](https://github.com/square/sharkey)| Sharkey 是OpenSSH管理证书使用的服务。Sharkey 分为客户端组件和服务端组件，服务端负责发布已签署的主机证书，客户端负责在机器上安装主机证书。 |335|
|[idcos/osinstall                      ](https://github.com/idcos/osinstall)| CloudBoot”(OSinstall)云装机平台，是金融云初创公司杭州云霁科技推出的一款X86服务器全自动装机工具，遵循Apache协议，完全开源免费。全自动构建物理机资源池，像创建虚拟机一样方便的安装物理机。 |299|

# 安全工具
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[inconshreveable/ngrok                      ](https://github.com/inconshreveable/ngrok)| ngrok 是一个反向代理，通过在公共的端点和本地运行的 Web 服务器之间建立一个安全的通道。ngrok 可捕获和分析所有通道上的流量，便于后期分析和重放。 |18297|
|[yahoo/gryffin                      ](https://github.com/yahoo/gryffin)| Gryffin 是雅虎开发的一个大规模 Web 安全扫描平台。它不是另外一个扫描器，其主要目的是为了解决两个特定的问题 —— 覆盖率和伸缩性。 |2003|
|[xiam/hyperfox                      ](https://github.com/xiam/hyperfox)| Hyperfox 是一个安全的工具用来代理和记录局域网中的 HTTP 和 HTTPS 通讯。 |1310|
|[sheepbao/gomitmproxy                      ](https://github.com/sheepbao/gomitmproxy)| GomitmProxy是想用golang语言实现的mitmproxy，主要实现http代理，目前实现了http代理和https抓包功能。 |277|

# 网络工具
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[containous/traefik                      ](https://github.com/containous/traefik)| Træfɪk 是一个新型的http反向代理、负载均衡软件，能轻易的部署微服务. 它支持多种后端 (Docker, Swarm, Mesos/Marathon, Consul, Etcd, Zookeeper, BoltDB, Rest API, file...) ,可以对配置进行自动化、动态的管理. |28027|
|[buger/gor                      ](https://github.com/buger/gor)| Gor 是用 Go 编写的简单 HTTP 流量复制工具，主要是为了从生产服务器返回流量到开发环境。使用 Gor 可以在实际的用户会话中测试代码。 |12436|
|[cyfdecyf/cow                      ](https://github.com/cyfdecyf/cow)| COW 是一个简化穿墙的 HTTP 代理服务器。它能自动检测被墙网站，仅对这些网站使用二级代理；支持多种协议：sock5、http、shadow、cow|8036|
|[google/seesaw                      ](https://github.com/google/seesaw)| Seesaw 是 Google 开源的一个基于 Linux 的负载均衡系统。Seesaw 包含基本的负载均衡特性，同时支持一些高级的功能，诸如：anycast, Direct Server Return (DSR), 支持多个 VLANs 和集中式配置。同时其设计的宗旨是易于维护。需要注意的是，尽管该项目挂靠在 Google 名下，但并非 Google 官方产品。 |4978|
|[mehrdadrad/mylg                      ](https://github.com/mehrdadrad/mylg)| myLG是一个开源的网络工具集，它包含了很多不同类型的网络诊断工具, 功能包括ping，trace， bgp， dns lookup， 端口扫描， 局域网网络发现，提供web界面, tcpdump等 |2293|
|[uber/tchannel                      ](https://github.com/uber/tchannel)| TChannel 是用于 RPC 的网络复用和成帧协议。             |1090|
|[GameXG/TcpRoute2                      ](https://github.com/GameXG/TcpRoute2)| TcpRoute, TCP 层的路由器。对于 TCP 连接自动从多个线路(允许任意嵌套)、多个域名解析结果中选择最优线路。TcpRoute2 是 golang 重写的版本。通过 socks5 代理协议对外提供服务。代理功能拆分成了独立的库，详细代理url格式级选项请参见 ProxyClient，目前支持直连、socks4、socks4a、socks5、http、https、ss 代理线路 |722|
|[jpillora/go-tcp-proxy                      ](https://github.com/jpillora/go-tcp-proxy)| go-tcp-proxy是一个简单的tcp代理， 可以用于tcp端口转发， 也可以用做http代理使用 |379|

# Web工具
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[yudai/gotty                      ](https://github.com/yudai/gotty)| GoTTY 是个简单的命令行工具，可以把 CLI 工具共享成 Web 应用。GoTTY 可以把终端作为 Web 应用共享。 |13682|
|[valyala/fasthttp                      ](https://github.com/valyala/fasthttp)|fasthttp 是 Go 的快速 HTTP 实现，当前在 1M 并发的生产环境使用非常成功，可以从单个服务器进行 100K qps 的持续连接。HTTP 服务器性能与 net/http 比较，fasthttp 比 net/http 快 10 倍 |11804|
|[gizak/termui                      ](https://github.com/gizak/termui)| Go语言编写的终端仪表盘                             |9661|
|[henrylee2cn/pholcus                      ](https://github.com/henrylee2cn/pholcus)| Pholcus（幽灵蛛）是一款纯Go语言编写的高并发、分布式、重量级爬虫软件，支持单机、服务端、客户端三种运行模式，拥有Web、GUI、命令行三种操作界面；规则简单灵活、批量任务并发、输出方式丰富（mysql/mongodb/csv/excel等）、有大量Demo共享；同时她还支持横纵向两种抓取模式，支持模拟登录和任务暂停、取消等一系列高级功能。 |6297|
|[lonelycode/tyk                      ](https://github.com/lonelycode/tyk)| Tyk 是一个开源的、轻量级的、快速可伸缩的 API 网关，支持配额和速度限制，支持认证和数据分析，支持多用户多组织，提供全 RESTful API。 |5328|
|[etsy/hound                      ](https://github.com/etsy/hound)| 快如闪电的代码搜索开源工具                            |4345|
|[Terry-Mao/goim                      ](https://github.com/Terry-Mao/goim)| goim 是一个支持集群的im及实时推送服务（支持websocket，http和tcp协议） |4009|
|[huichen/wukong                      ](https://github.com/huichen/wukong)| WuKong 是一个全文搜索引擎。功能特性有：高效索引和搜索（1M条微博500M数据28秒索引完，1.65毫秒搜索响应时间，19K搜索QPS）；支持中文分词（使用sego分词包并发分词，速度27MB/秒）；支持计算关键词在文本中的紧邻距离（token proximity）；支持计算BM25相关度；支持自定义评分字段和评分规则；支持在线添加、删除索引；支持持久存储；可实现分布式索引和搜索等 |3553|
|[afex/hystrix-go                      ](https://github.com/afex/hystrix-go)|    用来隔离远程系统调用， 第三方库调用 ，服务调用， 提供熔断机制，避免雪崩效应的库， Hystrix的go 版本。 注Hystrixs是Netflix开源的一个java库    |2407|
|[tus/tusd                      ](https://github.com/tus/tusd)|  实现文件上传的断点续传功能， 整套功能包含了协议实现，client， server。 client及server有多种语言的实现包括go， python， node等|1556|
|[codetainerapp/codetainer                      ](https://github.com/codetainerapp/codetainer)| Codetainer 可以让你创建基于浏览器上的代码运行沙箱，可方便的嵌入到你的 Web 应用中。你可以把它当成是 codepicnic.com 的开源克隆) . |975|
|[ga0/netgraph                      ](https://github.com/ga0/netgraph)| netgraph 是一个 Go 语言编写的跨平台的 B/S 架构的 HTTP 抓包工具，方便在 Linux 服务器上直接查看 HTTP 包。 |809|
|[andyxning/shortme                      ](https://github.com/andyxning/shortme)| 用Golang编写的URL短链接服务。                      |244|
|[hidu/pproxy                      ](https://github.com/hidu/pproxy)|http抓包代理程序,http协议调试工具 |237|

# Web框架
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[gin-gonic/gin                      ](https://github.com/gin-gonic/gin)| Gin 是一个用 Go 语言开发的 Web 框架，提供类 Martini 的 API，但是性能更好。因为有了 httprouter 性能提升了 40 倍之多。 |36433|
|[astaxie/beego                      ](https://github.com/astaxie/beego)| beego是一个用Go开发的应用框架，思路来自于tornado，路由设计来源于sinatra， |23525|
|[kataras/iris                      ](https://github.com/kataras/iris)| 通过Iris-Go，可以方便的帮助你来开发基于web的应用。简单来说：Iris-Go与国内大牛的BeeGo类似，但从其官方介绍的资料来看，Iris-Go的性能更优！ |17776|
|[labstack/echo                      ](https://github.com/labstack/echo)| Echo 是个快速的 HTTP 路由器（零动态内存分配），也是 Go 的微型 Web 框架。 |16793|
|[codegangsta/martini                      ](https://github.com/codegangsta/martini)| Martini 是一个非常新的 Go 语言的 Web 框架，使用 Go 的 net/http 接口开发，类似 Sinatra 或者 Flask 之类的框架，你可使用自己的 DB 层、会话管理和模板。 |10888|
|[hoisie/web                      ](https://github.com/hoisie/web)| web.go 跟 web.py 类似，但使用的是 Go 编程语言实现的 Web 应用开发框架。Go发布没多久该框架就诞生了，差不多是最早的Go框架。目前已经有段时间没有更新了。不过，该框架代码不多，其源码可以读一读。 |3440|
|[go-macaron/macaron                      ](https://github.com/go-macaron/macaron)| Macaron 是一个具有高生产力和模块化设计的 Go Web 框架。框架秉承了 Martini 的基本思想，并在此基础上做出高级扩展。 |2952|
|[gernest/utron                      ](https://github.com/gernest/utron)| utron 是一个 Go 语言轻量级的 MVC 框架，用于快速构建可伸缩以及可靠的数据库驱动的 Web 应用。 |2159|
|[olahol/melody                      ](https://github.com/olahol/melody)| Melody 是一个 Go 语言的微型 WebSocket 框架，基于 github.com/gorilla/websocket 开发， |1771|
|[henrylee2cn/faygo                      ](https://github.com/henrylee2cn/faygo)|Faygo 是一款快速、简洁的Go Web框架，可用极少的代码开发出高性能的Web应用程序（尤其是API接口）。只需定义 struct Handler，Faygo 就能自动绑定、验证请求参数并生成在线API文档。 |1503|
|[lunny/tango                      ](https://github.com/lunny/tango)| Tango，微内核可扩展的Go语言Web框架。同时支持函数和结构体作为执行体，插件丰富。 |835|
|[robfig/revel                      ](https://github.com/robfig/revel)| Revel 是 Go 语言的框架，其思路完全来自 Java 的 Play Framework。 |159|
|[go-baa/baa                      ](https://github.com/go-baa/baa)| Baa 一个简单高效的Go web开发框架。主要有路由、中间件，依赖注入和HTTP上下文构成。 |141|

# 区块链技术
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[ethereum/go-ethereum                      ](https://github.com/ethereum/go-ethereum)| go-ethereum客户端通常被称为geth，它是个命令行界面，执行在Go上实现的完整以太坊节点。通过安装和运行geth，可以参与到以太坊前台实时网络并进行以下操作：a. 挖掘真的以太币  b. 在不同地址间转移资金 c .创建合约，发送交易  d . 探索区块历史 e.很多其他功能 |25587|
|[hyperledger/fabric                      ](https://github.com/hyperledger/fabric)| Fabric是一个开源区块链实现，开发环境建立在VirtualBox虚拟机上，部署环境可以自建网络，也可以直接部署在BlueMix上，部署方式可传统可docker化，共识达成算法插件化，支持用Go和JavaScript开发智能合约，尤以企业级的安全机制和membership机制为特色。你要是不知道这些术语什么意思，就记住一点，Fabric之于区块链，很可能正如Hadoop之于大数据。 |9967|
|[chain/chain                      ](https://github.com/chain/chain)| **金融领域的区块链项目 **. Chain是由一家刚成立两年的美国创业公司Chain推出，是一个企业级的区块链平台架构，可以让机构构造从零开始更好的金融服务。Chain 开放标准在以下方面实现突破：• 全新的共识模型在不到一秒的时间里实现交易的最终完成，即便是交易量非常大也能支持;• 私密解决方案对区块链数据进行加密，并让相关对手方和监管者进行有选择的读取;• 智能合约框架和虚拟机支持简单的规则执行，以及进行键值存储的图灵完整程序; • 可伸缩的数据模型可以为网络参与者降低运行负荷; • 丰富的元数据层可支持满足KYC（了解你的客户）和 AML（反洗钱）要求 |1671|

# 其它
| 项目                                     | 简介                                       | Star数                                       |
| ---- | ------------------------------- | ---- |
|[gohugoio/hugo                      ](https://github.com/gohugoio/hugo)| Hugo是由Go语言实现的静态网站生成器；简单、易用、高效、易扩展、快速部署；相比于Hexo、Jekyll，hugo的优势是生成速度极快。 |42615|
|[mattermost/platform                      ](https://github.com/mattermost/platform)| mattermost 是一个 Slack 的开源替代品。Mattermost 采用 Go 语言开发，这是一个开源的团队通讯服务。为团队带来跨 PC 和移动设备的消息、文件分享，提供归档和搜索功能。 |17854|
|[grpc/grpc-go                      ](https://github.com/grpc/grpc-go)| GRPC 是一个高性能、开源和通用的 RPC 框架，面向移动和 HTTP/2 设计。目前提供 C、Java 和 Go 语言版本，分别是：grpc, grpc-java, grpc-go. 其中 C 版本支持 C, C++, Node.js, Python, Ruby, Objective-C, PHP 和 C# 支持.GRPC 基于 HTTP/2 标准设计，带来诸如双向流、流控、头部压缩、单 TCP 连接上的多复用请求等特。这些特性使得其在移动设备上表现更好，更省电和节省空间占用。 |10893|
|[Netflix/chaosmonkey                      ](https://github.com/Netflix/chaosmonkey)|     Chaos Monkey是netflix公司开源的一个用于服务可用性测试的工具，通过有计划的在生产系统制造真实的故障（如cpu负载高， 内存溢出，磁盘写满，服务器宕机等）来检测系统的可用性。 |8257|
|[apex/apex                      ](https://github.com/apex/apex)| 管理，部署aws lambda函数的工具， 支持用go语言编写lambda函数（注：目前aws官方不支持用go语言编写lambda函数，但是apex却可以变相支持） |8004|
|[rakyll/hey                      ](https://github.com/rakyll/hey)| Boom 是 google 一女工程师使用 Go 语言开发的类似 apache ab 的性能测试工具。相比 ab，boom跨平台性更好，而且更容易安装。 |7859|
|[visualfc/liteide                      ](https://github.com/visualfc/liteide)| LiteIDE是一款开源、跨平台的轻量级Go语言集成开发环境（IDE）。     |5925|
|[yinghuocho/firefly-proxy                      ](https://github.com/yinghuocho/firefly-proxy)| 穿墙工具。 GFW梯子。 提供客户端和服务端。支持多个平台， 包括linux， macos， windows ，android |4964|
|[qor/qor                      ](https://github.com/qor/qor)| Qor 是基于 Golang 开发的的CMS 一系列工具库，基于 Qor可以快速搭建网站的后台管理系统。Qor 的工作库包含：1，后台管理：可以对数据库进去 CURD 管理，支持一对一，一对多，多对多关联关系维护等等； 2，支持上传图片到云以及 filesystem，resize、crop 图片等等 ；3，Publish 发布系统，可以修改数据，并且经过检查后，再发布到正式环境中； 4，状态机，可以用于开发工作流的系统； 5，I18n，翻译，可以通过在 WEB 界面翻译，并将翻译保存到数据库中； 6，L10n，本地化，不同于翻译，他可以针对某个地区来对内容，或者数据结构进行本地化。7，Roles，权限管理； 8，Exchange，通过 Excel，CSV 导入导出数据； 9，Worker，后台任务管理，可用于跑定时任务等等 |4325|
|[golang/mobile                      ](https://github.com/golang/mobile)| Gomobile是一个应用于iOS和Android的优秀跨平台开发库，为开发者提供用于创建Android和iOS 移动平台代码的工具。 |4074|
|[getlantern/lantern                      ](https://github.com/getlantern/lantern)| Lantern是一个点对点科学上网软件。                     |2469|
|[vzex/dog-tunnel                      ](https://github.com/vzex/dog-tunnel)| 狗洞是一个高速的 P2P 端口映射工具，同时支持Socks5代理。 0.5版后开始开源，UDP底层基于开源库KCP重写，效率大大提高，在恶劣环境下优势明显。 同时提供非P2P版本（Lite版本），两端连接过程完全不依赖中间服务器，支持加密和登陆认证，自动重连，但是需要人为确保两端能正常连通（否则请使用默认的P2P版本） |1782|
|[prasmussen/glot                      ](https://github.com/prasmussen/glot)| glot 是可以可以在线运行各种编程语言代码片段的平台，项目采用 Haskell Script 、Go、Erlang 和 Shell 开发，运行环境基于 Docker 容器进行。 |1268|
|[yanyiwu/gojieba                      ](https://github.com/yanyiwu/gojieba)| "结巴"中文分词的Golang语言版本。                     |1014|
|[mikespook/gorbac                      ](https://github.com/mikespook/gorbac)| goRBAC 为 Go 语言应用提供了轻量级的基于角色的访问控制。        |998|
|[mailslurper/mailslurper                      ](https://github.com/mailslurper/mailslurper)| MailSlurper 是一个便携的 SMTP 邮件服务器，对本地和团队应用开发来说非常有用。MailSlurper 体积小运行快速，支持 SQLite, MSSQL 和 MySQL. 数据库。 |691|
|[xjdrew/kone                      ](https://github.com/xjdrew/kone)| 可用于家庭或者企业网络的透明代理，可用来翻墙等                  |621|
|[codeskyblue/gosuv                      ](https://github.com/codeskyblue/gosuv)| 进程管理， 类似于python的supervisord ， 提供了web管理界面 |591|
|[oikomi/FishChatServer2                      ](https://github.com/oikomi/FishChatServer2)| FishChat（鱼传——鱼传尺素）分布式可伸缩 IM 服务器，是一款纯 golang 编写优秀的即时通讯软件(IM), 它集合了市面上已有产品的优点, 并具备 智能硬件网关管理(学习QQ物联思想, 构思中)。 |466|
|[rafael-santiago/cherry                      ](https://github.com/rafael-santiago/cherry)| Cherry 是一个使用 Go 语言开发的 Web 聊天引擎。          |215|
|[robustirc/robustirc                      ](https://github.com/robustirc/robustirc)| RobustIRC 是不会有网络中断情况的 IRC。RobustIRC 主要特性：服务器不可用的时候不会有网络中断； 可以使用标准 IRC 客户端； 健壮，可以很好处理客户端和网络的连接问题 |126|


**[⬆ 返回顶部](#目录)**