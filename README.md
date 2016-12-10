看过awesome-go项目， 汇总了很多go开源项目。 但是awesome-go收集了太全了， 而且每个项目没有详细描述。 因此我自己根据go语言中文社区提供的资料，还有互联网企业架构设计中的常见组件分类， 共精心挑选了100多个开源项目（项目不限于在github开源的项目）， 分成以下十几个大类。 这个项目可以理解为互联网IT人打造的中文版awesome-go。这个项目初衷是帮助到那些想学习和借鉴优秀golang开源项目， 和在互联网架构设计时期望快速寻找合适轮子的人。

#  目录
- [监控系统](#监控系统)
- [容器技术](#容器技术)
- [PaaS工具](#PaaS工具)
- [大数据](#大数据)
- [微服务](#微服务)
- [持续集成与持续部署](#持续集成与持续部署)
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


| 序号   | 名称                              | 项目地址                                     | 简介                                       |
| ---- | ------------------------------- | ---------------------------------------- | ---------------------------------------- |
| 1    | OpenFalcon                      | https://github.com/open-falcon/of-release | OpenFalcon是一款小米开源的监控系统。功能：数据采集免配置：agent自发现、支持Plugin、主动推送模式; 容量水平扩展：生产环境每秒50万次数据收集、告警、存储、绘图，可持续水平扩展。告警策略自发现：Web界面、支持策略模板、模板继承和覆盖、多种告警方式、支持回调动作。告警设置人性化：支持最大告警次数、告警级别设置、告警恢复通知、告警暂停、不同时段不同阈值、支持维护周期，支持告警合并。历史数据高效查询：秒级返回上百个指标一年的历史数据。Dashboard人性化：多维度的数据展示，用户自定义Dashboard等功能。架构设计高可用：整个系统无核心单点，易运维，易部署。 |
| 2    | banshee                         | https://github.com/eleme/banshee         | 周期性指标的监控系统.                              |
| 3    | Kapacitor                       | https://github.com/influxdata/kapacitor  | Kapacitor 是一个开源框架，用来处理、监控和警告时间序列数据。      |
| 4    | Pome                            | https://github.com/rach/pome             | Pome 是 Postgres Metrics 的意思。Pome 是一个 PostgreSQL 的指标仪表器，用来跟踪你的数据库的健康状况。 |
| 5    | pingd                           | https://github.com/pinggg/pingd          | pingd 是世界上最简单的监控服务，使用 golang 编写。软件支持 IPv6，但是服务器不支持. pingd 允许同时 ping 上千个 IPs，在此期间还可以管理监控的主机。用户提供主机名或者 IP，还有用户邮箱地址，就可以使用 3 个生成 URLs 来开启，停止或者删除你的追踪。每当你的服务器停机或者后台在线都会发送通知，还包含控制 URLs。 |
| 6    | actiontech zabbix mysql monitor | https://github.com/actiontech/actiontech_zabbix_mysql_monitor | percona monitoring plugins zabbix 的 Go 语言版本，是由 爱可生 公司开源的 MySQL 监控插件和模板，整合上百个性能监控指标，支持Low Level Discovery 自动发现多实例环境，支持performance_schema |
| 7    | rtop                            | https://github.com/rapidloop/rtop        | top 是一个简单的无代理的远程服务器监控工具，基于 SSH 连接进行工作。无需在被监控的服务器上安装任何软件。rtop 直接通过 SSH 连接到待监控服务器，然后执行命令来收集监控数据。rtop 每几秒钟就自动更新监控数据，类似其他 *top 命令 |
| 8    | Prometheus                      | https://github.com/prometheus/prometheus | Prometheus 是一个开源的服务监控系统和时间序列数据库， 提供监控数据存储，展示，告警等功能 |
| 9    | bosun                           | https://github.com/bosun-monitor/bosun   | 专业的跨平台开源系统监控项目，go语言编写，灵活的模板和表达式配合上各种collector可以监控任何应用或系统级的运行数据，比 zabbix更轻量级、更易入手和更适合定制。 |
| 10   | urlooker                        | https://github.com/urlooker              | 监控web服务可用性及访问质量，采用go语言编写，易于安装和二次开发. 支持一下特性： 返回状态码检测;   页面响应时间检测;  页面关键词匹配检测;   带cookie访问;  agent多机房部署，指定机房访问;  检测结果支持向open-falcon推送;  支持短信和邮件告警 |
| 11   | satellite                       | https://github.com/gravitational/satellite | 用于监测kubernetes健康状态的一个工具／库。 其特点是：轻量级定期测试， 高可用性和弹性网络分区， 无单点故障， 以时间序列的格式存储监控数据。 |
| 12   | checkup                         | https://github.com/sourcegraph/checkup   | 一个分布式的无锁的站点健康状态检查工具。 支持检查http， tcp， dns等的状态 并可将结果保存在s3。 自带了一个美观的界面。 |
| 13   | zabbixctl                       | https://github.com/kovetskiy/zabbixctl   | Zabbixctl 是采用Zabbix服务API的命令行工具，它提供了有效的方式去查询和处理trigger 状态、主机最新数据和用户组。 |
| 14   | cloudinsight-agent              | https://github.com/cloudinsight/cloudinsight-agent/ | 提供可视化监控的saas平台cloudinsight开源的一个监控客户端。 Cloudinsight 探针可以收集它所在操作系统的各种指标，然后发送到 Cloudinsight 后端服务 |
| 15   | owl                             | https://github.com/TalkingData/owl       | OWL是TalkingData公司推出的一款开源分布式监控系统, 演示环境http://54.223.127.87/， 登录账号密码demo/demo |

# 容器技术
| 序号   | 名称         | 项目地址                                    | 简介                                       |
| ---- | ---------- | --------------------------------------- | ---------------------------------------- |
| 1    | SwarmKit   | https://github.com/docker/swarmkit      | SwarmKit 是Docker公司开源的Docker集群管理和容器编排工具，其主要功能包括节点发现、基于raft算法的一致性和任务调度等。 |
| 2    | DaoliNet   | https://github.com/daolinet/daolinet    | DaoliNet是一个软件定义网络(SDN)系统，其设计目的是为Docker容器提供动态、高效的链接。在Docker容器中，微服务工作负载具有轻量且短暂的性质，DaoliNet恰好适用于这种性质。 |
| 3    | Harbor     | https://github.com/vmware/harbor        | 容器应用的开发和运行离不开可靠的镜像管理。从安全和效率等方面考虑，部署在私有环境内的Registry是非常必要的。Project Harbor是由VMware公司中国团队为企业用户设计的Registry server开源项目，包括了权限管理(RBAC)、LDAP、审计、管理界面、自我注册、HA等企业必需的功能，同时针对中国用户的特点，设计镜像复制和中文支持等功能 |
| 4    | REX-Ray    | https://github.com/emccode/rexray       | REX-Ray 是一个 EMC {code} 团队领导的开源项目，为 Docker、Mesos 及其他容器运行环境提供持续的存储访问。其设计旨在囊括通用存储、虚拟化和云平台，提供高级的存储功能。 |
| 5    | Clair      | https://github.com/coreos/clair         | Clair 是一个容器漏洞分析服务。它提供一个能威胁容器漏洞的列表，并且在有新的容器漏洞发布出来后会发送通知给用户。 |
| 6    | Weave      | https://github.com/zettio/weave         | Weave 创建一个虚拟网络并连接到部署在多个主机上的 Docker 容器。   |
| 7    | Rocket     | https://github.com/coreos/rkt           | Rocket （也叫 rkt）是 CoreOS 推出的一款容器引擎，和 Docker 类似，帮助开发者打包应用和依赖包到可移植容器中，简化搭环境等部署工作。Rocket 和 Docker 不同的地方在于，Rocket 没有 Docker 那些为企业用户提供的“友好功能”，比如云服务加速工具、集群系统等。反过来说，Rocket 想做的，是一个更纯粹的业界标准。 |
| 8    | libnetwork | https://github.com/docker/libnetwork    | Libnetwork 提供一个原生 Go 实现的容器连接，是容器的网络。libnetwork 的目标是定义一个健壮的容器网络模型（Container Network Model），提供一个一致的编程接口和应用程序的网络抽象。 |
| 9    | Wormhole   | https://github.com/vishvananda/wormhole | WWormhole 是一个能识别命名空间的由 Socket 激活的隧道代理。可以让你安全的连接在不同物理机器上的 Docker 容器。可以用来完成一些有趣的功能，例如连接运行在容器本机的服务或者在连接后创建按需的服务。 |
| 10   | Shipyard   | https://github.com/shipyard/shipyard    | Shipyard 是一个基于 Web 的 Docker 管理工具，支持多 host，可以把多个 Docker host 上的 containers 统一管理；可以查看 images，甚至 build images；并提供 RESTful API 等等。 Shipyard 要管理和控制 Docker host 的话需要先修改 Docker host 上的默认配置使其支持远程管理。 |
| 11   | Docker     | https://github.com/docker/docker        | Docker 是一个开源的应用容器引擎，让开发者可以打包他们的应用以及依赖包到一个可移植的容器中，然后发布到任何流行的 Linux 机器上，也可以实现虚拟化。容器是完全使用沙箱机制，相互之间不会有任何接口（类似 iPhone 的 app）。几乎没有性能开销,可以很容易地在机器和数据中心中运行。最重要的是,他们不依赖于任何语言、框架或包装系统。 |
| 12   | scope      | https://github.com/weaveworks/scope     | 一个docker&kubernetes的管理，监控可视化工具， 可以看到容器间的拓扑关系和tcp通信 |
| 13   | habitus    | https://github.com/cloud66/habitus      | 一个快速实现docker build 流程的工具， 支持复杂的docker build流程，实现多个dockerfile的build流程，典型应用如将需要静态编译的程序，如go， java这类程序在一个docker build编译好之后，得到的二进制包用到后续的build流程 |
| 14   | sextant    | https://github.com/k8sp/sextant         | sextant 提供了可以通过PXE全自动化安装初始化一个CoreOS+kubernetes集群。 |

# PaaS工具
| 序号   | 名称                 | 项目地址                                     | 简介                                       |
| ---- | ------------------ | ---------------------------------------- | ---------------------------------------- |
| 1    | Kel                | https://github.com/kelproject            | Kel 是一个开源的基于 Kubernetes 构建的 PaaS 系统，采用 Python 和 Go 语言开发。Kel 可简化管理 Web 应用发布和托管整个软件生命周期。Kel 帮助开发和运维人员轻松管理他们的应用架构，通过一组工具和组件让 K8S 使用非常简单。 |
| 2    | CloudFoundry-Mesos | https://github.com/mesos/cloudfoundry-mesos | Cloud Foundry-Mesos框架由华为与Mesosphere的工程师合作完成，能够为应用提供安全可靠的、可伸缩、可扩展的云端运行环境，并且应用能够 享用Cloud Foundry生态圈内各类丰富的服务资源。企业能够通过Cloud Foundry开发云应用，并通过Cloud Foundry-Mesos将应用部署到DCOS上，使应用能够与DCOS上安装的其他服务及应用框架共享资源，实现资源利用率最大化，能够大幅降低企业 数据中心运营成本。DCOS能够运行在虚拟和物理环境上，能够支持Linux（以及很快支持Windows），并可适用于私有云、公有云及混合云环境。 |
| 3    | Flynn              | https://github.com/github/flynn          | Flynn 是一个开源的 PaaS 系统，由 Docker 开发。采用 Go 语言编写。支持数据库包括 Postgres、Redis 和 MongoDB. Flynn 使用完全组件化模块化的设计，任何一个组件和模块都可以独立的进行替换。 |
| 4    | DINP               | https://git.oschina.net/cnperl/dinp-server | DINP是又一个基于Docker开发的PaaS平台。               |
| 5    | Kubernetes         | https://github.com/kubernetes/kubernetes | Kubernetes 是来自 Google 云平台的开源容器集群管理系统。基于 Docker 构建一个容器的调度服务。该系统可以自动在一个容器集群中选择一个工作容器供使用。其核心概念是 Container Pod。 |
| 6    | Tsuru              | https://github.com/tsuru/tsuru           | 在 Tsuru 的 PaaS 服务下，你可以选择自己的编程语言，选择使用 SQL 或者 NoSQL 数据库，memcache、redis、等等许多服务，甚至与你可以使用 Git 版本控制工具来上传你应用。 |
| 7    | atlantis           | https://github.com/ooyala/atlantis       | Atlantis 是一款基于 Docker，使用 Go 编写，为 HTTP 应用准备的开源 PaaS。Atlantis 可以在路由请求中轻松的构建和部署应用到容器。Atlantis 在 Ooyala 的新应用中得到了很广泛的应用。 |

# 大数据
| 序号   | 名称       | 项目地址                                   | 简介                                       |
| ---- | -------- | -------------------------------------- | ---------------------------------------- |
| 1    | MLF      | https://github.com/huichen/mlf         | 弥勒佛项目是一个大数据机器学习框架。具有为处理大数据优化，可随业务增长scale up，模型的训练和使用都可以作为library或者service整合到在生产系统中，具有丰富的模型，高度可扩展，高度可读性，适合初学者进行大数据模型的学习等特点 |
| 2    | Glow     | https://github.com/chrislusf/glow      | glow 是使用 Go 编写的易用分布式计算系统，是 Hadoop Map Reduce，Spark，Flint，Samza 等等的替代品。Glow 的目标是提供一个库，可以在并行线程或者分布式集群机器中进行更简单计算。 |
| 3    | goml     | https://github.com/cdipaolo/goml       | 机器学习的库, 包含了许多工具，能让你以在线方式学习其频道的数据内容。      |
| 4    | Golearn  | https://github.com/sjwhitworth/golearn | GoLearn实现了熟悉的Scikit-learn 适应/预测界面，可实现快速预估测试和交换。GoLearn是一个成熟的项目，它提供了交叉验证和训练/测试等辅助功能。 |
| 5    | Gorgonia | https://github.com/chewxy/gorgonia     | 这个机器学习资料库完全是用Go语言编写而成，据其开发者“chewxy”称能“ 提供动态建立神经网络及相关算法必需条件 。” |

# 微服务
| 序号   | 名称         | 项目地址                                   | 简介                                       |
| ---- | ---------- | -------------------------------------- | ---------------------------------------- |
| 1    | kite       | https://github.com/koding/kite         | 一个基于go语言的微服务框架, Kite是Koding公司内部的一个框架, 该框架提供服务发现，多种认证功能，服务端通过RPC进行通信，同时还提供了websocket的js库，方便浏览器于服务器间进行通信。 |
| 2    | goa        | https://github.com/goadesign/goa       | Goa 是一款用 Go 用于构建微服务的框架，采用独特的设计优先的方法。     |
| 3    | Go-kit     | https://github.com/go-kit/kit          | Go-kit 是一个 Go 语言的分布式开发包，用于开发微服务。         |
| 4    | Hprose     | https://github.com/andot/hprose        | Hprose 是高性能远程对象服务引擎（High Performance Remote Object Service Engine）的缩写 —— 微服务首选引擎。它是一个先进的轻量级的跨语言跨平台面向对象的高性能远程动态通讯中间件。它不仅简单易用，而且功能强大。你只需要稍许的时间去学习，就能用它轻松构建跨语言跨平台的分布式应用系统了。 |
| 5    | Gizmo      | https://github.com/NYTimes/gizmo       | 纽约时报开源的go微服务工具.提供如下特性:标准化配置和日志;可配置策略的状态监测端点;用于管理 pprof 端点和日志级别的配置;结构化日志，提供基本请求信息;端点的有用度量;优雅的停止服务; 定义期待和词汇的基本接口 |
| 6    | hystrix-go | https://github.com/afex/hystrix-go     | 用来隔离远程系统调用， 第三方库调用 ，服务调用， 提供熔断机制，避免雪崩效应的库， Hystrix的go 版本。 注Hystrixs是Netflix开源的一个java库 |
| 7    | gateway    | https://github.com/fagongzi/gateway    | Gateway是一个使用go实现的基于HTTP的API 网关。**特性** ：API 聚合 ; 流控;  熔断; 负载均衡; 健康检查;  监控;  消息路由;  后端管理WebUI .  **能做什么**：规划更友好的URL给调用者。聚合多个API的结果返回给API调用者，利于移动端，后端可以实现原子接口。保护后端API服务不会被突发异常流量压垮。提供熔断机制，使得后端API Server具备自我恢复能力。借助消息路由能力，实现灰度发布，AB测试。 |
| 8    | fabio      | https://github.com/eBay/fabio          | fabio 是 ebay 团队用 golang 开发的一个快速、简单零配置能够让 consul 部署的应用快速支持 http(s) 的负载均衡路由器。这里有一篇中文文章http://dockone.io/article/1567介绍了如何用fabio＋consul实现服务发现，负载均衡，并阐述了原理， 最后还有demo程序 |
| 9    | appdash    | https://github.com/sourcegraph/appdash | go版本的分布式应用跟踪系统， 基于google dapper的原理构建     |

# 持续集成与持续部署

| 序号   | 名称      | 项目地址                                | 简介                                       |
| ---- | ------- | ----------------------------------- | ---------------------------------------- |
| 1    | Cyclone | https://github.com/caicloud/cyclone | Cyclone 是一个打造容器工作流的云原生持续集成持续发布平台，简单易用，使用 Go 语言开发，有详尽的中文文档 |
| 2    | Drone   | https://github.com/drone/drone      | Drone 是一个基于 Docker 的持续发布平台，使用 Go 语言开发    |

# 数据库技术
| 序号   | 名称                | 项目地址                                     | 简介                                       |
| ---- | ----------------- | ---------------------------------------- | ---------------------------------------- |
| 1    | BuntDB            | github.com/tidwall/buntdb                | 是纯Go开发的、低层级的（low-level）的、可嵌入的key/value内存数据库（IMDB），数据持久化存储，遵从ACID，支持自定义索引和geospatial 数据。 |
| 2    | Cockroach         | https://github.com/cockroachdb/cockroach | CockroachDB (蟑螂数据库）是一个可伸缩的、支持地理位置处理、支持事务处理的数据存储系统。CockroachDB 提供两种不同的的事务特性，包括快照隔离（snapshot isolation，简称SI）和顺序的快照隔离（SSI）语义，后者是默认的隔离级别。 |
| 3    | qb-go             | https://github.com/aacanakin             | qb是用来让使更容易使用数据库的go语言的数据库工具包。它受Python最喜欢的ORM SQLAlchemy的启发，既是一个ORM，也是一个查询生成器。它在表达api和查询构建东西的情形下是相当模块化的。 |
| 4    | GoshawkDB         | https://github.com/goshawkdb             | GoshawkDB 是一个采用 Go 语言开发支持多平台的分布式的对象存储服务，支持事务以及容错。GoshawkDB 的事务控制是在客户端完成的。GoshawkDB 服务器端使用 AGPL 许可，而 Go 语言客户端使用 Apache 许可证 |
| 5    | Codis             | https://github.com/wandoulabs/codis      | odis 是一个分布式 Redis 解决方案, 对于上层的应用来说, 连接到 Codis Proxy 和连接原生的 Redis Server 没有明显的区别 (不支持的命令列表), 上层应用可以像使用单机的 Redis 一样使用, Codis 底层会处理请求的转发, 不停机的数据迁移等工作, 所有后边的一切事情, 对于前面的客户端来说是透明的, 可以简单的认为后边连接的是一个内存无限大的 Redis 服务. |
| 6    | Cayley            | https://github.com/google/cayley         | Cayley 是 Google 的一个开源图(Graph)数据库，其灵感来自于 Freebase 和 Google 的 Knowledge Graph 背后的图数据库。 |
| 7    | Redigo            | https://github.com/garyburd/redigo       | Redigo 是 Redis 数据库的 Go 客户端。              |
| 8    | redis-go-cluster  | https://github.com/chasex/redis-go-cluster | redis-go-cluster 是基于 Redigo 实现的 Golang Redis 客户端。redis-go-cluster 可以在本地缓存 slot 信息，并且当集群修改的时候会自动更新。此客户端管理每个节点连接池，使用 goroutine 来尽可能的并发执行，达到了高效，低延迟。 |
| 9    | Dgraph            | https://github.com/dgraph-io/dgraph      | dgraph 是可扩展的，分布式的，低延迟图形数据库。DGraph 的目标是提供 Google 生产水平的规模和吞吐量，在超过TB的结构数据里，未用户提供足够低延迟的实时查询。DGraph 支持 GraphQL 作为查询语言，响应 JSON。 |
| 10   | DegDB             | https://github.com/degdb/degdb           | DegDB 是分布式的经济图数据库。                       |
| 11   | Vitess            | https://github.com/youtube/vitess        | outube出品的开源分布式MySQL工具集Vitess，自动分片存储MySQL数据表，将单个SQL查询改写为分布式发送到多个MySQL Server上，支持行缓存（比MySQL本身缓存效率高），支持复制容错，已用于Youtube生产环境 |
| 12   | xuncache          | https://github.com/sun8911879/xuncache   | xuncache 是免费开源的NOSQL(内存数据库) 采用golang开发,简单易用而且 功能强大(就算新手也完全胜任)、性能卓越能轻松处理海量数据,可用于缓存系统. |
| 13   | pgweb             | https://github.com/sosedoff/pgweb        | gweb 是一个采用 Go 语言开发的基于 Web 的 PostgreSQL 管理系统。 |
| 14   | Orchestrator      | https://github.com/outbrain/orchestrator | MySQL 复制拓扑可视化工具                          |
| 15   | mysql-schema-sync | https://github.com/hidu/mysql-schema-sync | mysql-schema-sync 是一款使用go开发的、跨平台的、绿色无依赖的 MySQL 表结构自动同步工具。用于将线上(其他环境)数据库结构变化同步到测试（本地）环境! |
| 16   | TiDB              | https://github.com/pingcap/tidb          | TiDB 是国内 PingCAP 团队开发的一个分布式 SQL 数据库。其灵感来自于 Google 的 F1, TiDB 支持包括传统 RDBMS 和 NoSQL 的特性。 |
| 17   | kingshard         | https://github.com/flike/kingshard       | 一个高性能的mysql中间件， 支持读写分离， 数据分片， 安全审计等功能    |
| 18   | influxdb          | https://github.com/influxdata/influxdb   | 一个可以水平扩展的时间序列数据库， 内建http api， 支持对数据打tag，灵活的查询策略和数据的实时查询，支持类sql语句进行查询 |



# 存储技术
| 序号   | 名称        | 项目地址                                   | 简介                                       |
| ---- | --------- | -------------------------------------- | ---------------------------------------- |
| 1    | Torus     | https://github.com/coreos/torus        | Torus是一种针对容器集群量身打造的存储系统，可以为通过Kubernetes编排和管理的容器集群提供可靠可扩展的存储。这是继etcd、rkt、flannel，以及CoreOS Linux之后CoreOS发布的另一个开源产品。 |
| 2    | Afero     | https://github.com/spf13/afero         | Afero 是一个文件系统框架，提供一个简单、统一和通用的 API 和任何文件系统进行交互，作为抽象层还提供了界面、类型和方法。Afero 的界面十分简洁，设计简单，舍弃了不必要的构造函数和初始化方法。Afero 作为一个库还提供了一组可交互操作的后台文件系统，这样在与 Afero 协作时，还可以保留 os 和 ioutil 软件包的功能和好处。 |
| 3    | REX-Ray   | https://github.com/emccode/rexray      | REX-Ray 是一个 EMC {code} 团队领导的开源项目，为 Docker、Mesos 及其他容器运行环境提供持续的存储访问。其设计旨在囊括通用存储、虚拟化和云平台，提供高级的存储功能。 |
| 4    | SeaweedFS | https://github.com/chrislusf/seaweedfs | SeaweedFS 是简单，高伸缩性的分布式文件系统，包含两部分：存储数十亿的文件；快速为文件服务。SeaweedFS 作为支持全 POSIX 文件系统语义替代，Seaweed-FS 选择仅实现 key-file 的映射，类似 "NoSQL"，也可以说是 "NoFS"。 |
| 5    | bfs       | https://github.com/Terry-Mao/bfs       | bfs 是使用 Go 编写的分布式文件系统（小文件存储）。            |
| 6    | IPFS      | https://github.com/ipfs/go-ipfs        | IPFS 是分布式文件系统，寻求连接所有计算机设备的相同文件系统。在某些方面，这很类似于原始的 Web 目标，但是 IPFS 最终会更像单个比特流群交换的 git 对象。IPFS ＝ InterPlanetary File System |


# 分布式系统
| 序号   | 名称        | 项目地址                                   | 简介                                       |
| ---- | --------- | -------------------------------------- | ---------------------------------------- |
| 1    | Confd     | https://github.com/kelseyhightower     | Confd是一个轻量级的配置管理工具。通过查询Etcd，结合配置模板引擎，保持本地配置最新，同时具备定期探测机制，配置变更自动reload。 |
| 2    | zerg      | https://github.com/huichen/zerg        | 基于docker的分布式爬虫服务                         |
| 3    | Doorman   | https://github.com/youtube/doorman     | Doorman 是一个客户端速率限制的解决方案，客户端与共享资源进行通讯，包括数据库、gRPC 服务、RESTful API 等等可使用 Doorman 来限制对资源的调用。Doorman 使用 Go 语言开发，使用 gRPC 的通讯协议。其高可用特性需要一个分布式的锁管理器，当前支持 etcd，也可使用 Zookeeper 替代。 |
| 4    | mgmt      | https://github.com/purpleidea/mgmt     | mgmt 是一个分布式的，事件驱动的配置管理工具。该工具支持并行执行，其 librarification 作为新的及已存在的软件的基础管理工具。 |
| 5    | Yoke      | https://github.com/nanopack/yoke       | Yoke 是 Postgres 的高可用集群，具有自动切换和自动集群恢复。Postgres冗余/自动故障转移解决方案，提供一个高可用PostgreSQL集群的简单管理。 |
| 6    | SeaweedFS | https://github.com/chrislusf/seaweedfs | SeaweedFS 是简单，高伸缩性的分布式文件系统，包含两部分：存储数十亿的文件；快速为文件服务。SeaweedFS 作为支持全 POSIX 文件系统语义替代，Seaweed-FS 选择仅实现 key-file 的映射，类似 "NoSQL"，也可以说是 "NoFS"。 |
| 7    | Glow      | https://github.com/chrislusf/glow      | Glow 是使用 Go 编写的易用分布式计算系统，是 Hadoop Map Reduce，Spark，Flint，Samza 等等的替代品。Glow 的目标是提供一个库，可以在并行线程或者分布式集群机器中进行更简单计算。 |
| 8    | Nomad     | https://github.com/hashicorp/nomad     | Nomad 是一个集群管理器和调度器，专为微服务和批量处理工作流设计。Nomad 是分布式，高可用，可扩展到跨数据中心和区域的数千个节点。 |
| 9    | dcmp      | https://github.com/silenceper/dcmp     | DCMP是分布式配置管理平台。提供了一个etcd的管理界面，可通过界面修改配置信息，借助confd可实现配置文件的同步。 |
| 10   | gleam     | https://github.com/chrislusf/gleam     | 此处是一个通过Go和LuaJIT编写的快速和可扩展的分布式map/reduce系统，很好的将Go的高并发性与Luajit高性能相结合，可独立运行或用于分布式计算。 |



# 消息系统
| 序号   | 名称           | 项目地址                                     | 简介                                       |
| ---- | ------------ | ---------------------------------------- | ---------------------------------------- |
| 1    | KiteQ        | https://github.com/blackbeans/kiteq      | KiteQ 是一个基于 go + protobuff 实现的多种持久化方案的 mq 框架（消息队列）。 |
| 2    | NSQ          | https://github.com/bitly/nsq             | NSQ 是无中心设计、节点自动注册和发现的开源消息系统。可作为内部通讯框架的基础，易于配置和发布。 |
| 3    | kingtask     | https://github.com/kingsoft-wps/kingtask | kingtask是一个由Go开发的轻量级的异步定时任务系统。支持定时的异步任务。 支持失败重试机制，重试时刻和次数可自定义。 任务执行结果可查询。 |
| 4    | Go Machinery | https://github.com/RichardKnop/machinery | Machinery 是一个 Go 语言的异步任务队列和作业队列，基于分布式消息传递。类似 Python 的 Celery 框架。 |
| 5    | kaca         | https://github.com/scottkiss/kaca        | kaca 是用 golang 语言开发的基于 websocket 协议的消息发布/订阅系统。 |

# 服务器管理
| 序号   | 名称        | 项目地址                                     | 简介                                       |
| ---- | --------- | ---------------------------------------- | ---------------------------------------- |
| 1    | Sharkey   | https://github.com/square/sharkey        | Sharkey 是OpenSSH管理证书使用的服务。Sharkey 分为客户端组件和服务端组件，服务端负责发布已签署的主机证书，客户端负责在机器上安装主机证书。 |
| 2    | OSinstall | https://github.com/idcos/osinstall       | CloudBoot”(OSinstall)云装机平台，是金融云初创公司杭州云霁科技推出的一款X86服务器全自动装机工具，遵循Apache协议，完全开源免费。全自动构建物理机资源池，像创建虚拟机一样方便的安装物理机。 |
| 3    | ssh2go    | https://github.com/karfield              | ssh2go 是对libssh的golang 封装。libssh是SSH的代码库，同时支持服务端和客户端，日常所见的ssh, sshd, scp, sftp均基于libssh。ssh2go是对libssh的Go语言绑定， 100%的libssh接口都可用，同时集成示例，方便参考。 |
| 4    | Gooverssh | https://github.com/scottkiss/gooverssh   | gooverssh 是基于gosshtool的一个ssh开发包开发的一个基于ssh本地端口转发服务小应用，可以方便突破一些网络限制，如通过ssh代理访问内网数据库服 |
| 5    | gosshtool | https://github.com/scottkiss/gosshtool   | gosshtool provide some useful functions for ssh client in golang.implemented using golang.org/x/crypto/ssh.go语言中提供ssh相关操作，支持ssh本地端口转发服务 |
| 6    | teleport  | https://github.com/gravitational/teleport | teleport 是 初创公司Gravitational 的一款基于ssh和https的远程管理linux 集群服务器的工具， 其特点是支持双重校验登陆；操作记录回放；session共享，便于协作排障；自动发现集群的服务器和容器 |

# 安全工具
| 序号   | 名称          | 项目地址                                     | 简介                                       |
| ---- | ----------- | ---------------------------------------- | ---------------------------------------- |
| 1    | gomitmproxy | https://github.com/sheepbao/gomitmproxy  | GomitmProxy是想用golang语言实现的mitmproxy，主要实现http代理，目前实现了http代理和https抓包功能。 |
| 2    | Hyperfox    | https://github.com/xiam/hyperfox         | Hyperfox 是一个安全的工具用来代理和记录局域网中的 HTTP 和 HTTPS 通讯。 |
| 3    | Gryffin     | https://github.com/yahoo/gryffin         | Gryffin 是雅虎开发的一个大规模 Web 安全扫描平台。它不是另外一个扫描器，其主要目的是为了解决两个特定的问题 —— 覆盖率和伸缩性。 |
| 4    | ngrok       | https://github.com/inconshreveable/ngrok | ngrok 是一个反向代理，通过在公共的端点和本地运行的 Web 服务器之间建立一个安全的通道。ngrok 可捕获和分析所有通道上的流量，便于后期分析和重放。 |


# 网络工具
| 序号   | 名称           | 项目地址                                     | 简介                                       |
| ---- | ------------ | ---------------------------------------- | ---------------------------------------- |
| 1    | DaoliNet     | https://github.com/daolinet/daolinet     | DaoliNet是一个软件定义网络(SDN)系统，其设计目的是为Docker容器提供动态、高效的链接。在Docker容器中，微服务工作负载具有轻量且短暂的性质，DaoliNet恰好适用于这种性质。 |
| 2    | Seesaw       | https://github.com/google/seesaw         | Seesaw 是 Google 开源的一个基于 Linux 的负载均衡系统。Seesaw 包含基本的负载均衡特性，同时支持一些高级的功能，诸如：anycast, Direct Server Return (DSR), 支持多个 VLANs 和集中式配置。同时其设计的宗旨是易于维护。需要注意的是，尽管该项目挂靠在 Google 名下，但并非 Google 官方产品。 |
| 3    | TcpRoute2    | https://github.com/GameXG/TcpRoute2      | TcpRoute, TCP 层的路由器。对于 TCP 连接自动从多个线路(允许任意嵌套)、多个域名解析结果中选择最优线路。TcpRoute2 是 golang 重写的版本。通过 socks5 代理协议对外提供服务。代理功能拆分成了独立的库，详细代理url格式级选项请参见 ProxyClient，目前支持直连、socks4、socks4a、socks5、http、https、ss 代理线路 |
| 4    | Gor          | https://github.com/buger/gor             | Gor 是用 Go 编写的简单 HTTP 流量复制工具，主要是为了从生产服务器返回流量到开发环境。使用 Gor 可以在实际的用户会话中测试代码。 |
| 5    | Traefik      | https://github.com/containous/traefik    | Træfɪk 是一个新型的http反向代理、负载均衡软件，能轻易的部署微服务. 它支持多种后端 (Docker, Swarm, Mesos/Marathon, Consul, Etcd, Zookeeper, BoltDB, Rest API, file...) ,可以对配置进行自动化、动态的管理. |
| 6    | TChannel     | https://github.com/uber/tchannel         | TChannel 是用于 RPC 的网络复用和成帧协议。             |
| 7    | go-tcp-proxy | https://github.com/jpillora/go-tcp-proxy | go-tcp-proxy是一个简单的tcp代理， 可以用于tcp端口转发， 也可以用做http代理使用 |
| 8    | myLG         | https://github.com/mehrdadrad/mylg       | myLG是一个开源的网络工具集，它包含了很多不同类型的网络诊断工具, 功能包括ping，trace， bgp， dns lookup， 端口扫描， 局域网网络发现，提供web界面, tcpdump等 |

# Web工具
| 序号   | 名称           | 项目地址                                     | 简介                                       |
| ---- | ------------ | ---------------------------------------- | ---------------------------------------- |
| 1    | Tyk          | https://github.com/lonelycode/tyk        | Tyk 是一个开源的、轻量级的、快速可伸缩的 API 网关，支持配额和速度限制，支持认证和数据分析，支持多用户多组织，提供全 RESTful API。 |
| 2    | Shortme      | https://github.com/andyxning             | 用Golang编写的URL短链接服务。                      |
| 3    | WuKongSearch | https://github.com/huichen/wukong        | WuKong 是一个全文搜索引擎。功能特性有：高效索引和搜索（1M条微博500M数据28秒索引完，1.65毫秒搜索响应时间，19K搜索QPS）；支持中文分词（使用sego分词包并发分词，速度27MB/秒）；支持计算关键词在文本中的紧邻距离（token proximity）；支持计算BM25相关度；支持自定义评分字段和评分规则；支持在线添加、删除索引；支持持久存储；可实现分布式索引和搜索等 |
| 4    | Pholcus      | https://github.com/henrylee2cn/pholcus   | Pholcus（幽灵蛛）是一款纯Go语言编写的高并发、分布式、重量级爬虫软件，支持单机、服务端、客户端三种运行模式，拥有Web、GUI、命令行三种操作界面；规则简单灵活、批量任务并发、输出方式丰富（mysql/mongodb/csv/excel等）、有大量Demo共享；同时她还支持横纵向两种抓取模式，支持模拟登录和任务暂停、取消等一系列高级功能。 |
| 5    | Codetainer   | https://github.com/codetainerapp/codetainer | Codetainer 可以让你创建基于浏览器上的代码运行沙箱，可方便的嵌入到你的 Web 应用中。你可以把它当成是 codepicnic.com 的开源克隆) . |
| 6    | GoTTY        | https://github.com/yudai/gotty           | GoTTY 是个简单的命令行工具，可以把 CLI 工具共享成 Web 应用。GoTTY 可以把终端作为 Web 应用共享。 |
| 7    | TermUI       | https://github.com/gizak/termui          | Go语言编写的终端仪表盘                             |
| 8    | Hound        | https://github.com/etsy/hound            | 快如闪电的代码搜索开源工具                            |
| 9    | goim         | https://github.com/Terry-Mao/goim        | goim 是一个支持集群的im及实时推送服务（支持websocket，http和tcp协议） |
| 10   | fasthttp     | https://github.com/valyala/fasthttp      | asthttp 是 Go 的快速 HTTP 实现，当前在 1M 并发的生产环境使用非常成功，可以从单个服务器进行 100K qps 的持续连接。HTTP 服务器性能与 net/http 比较，fasthttp 比 net/http 快 10 倍 |
| 11   | netgraph     | https://github.com/ga0/netgraph          | netgraph 是一个 Go 语言编写的跨平台的 B/S 架构的 HTTP 抓包工具，方便在 Linux 服务器上直接查看 HTTP 包。 |
| 12   | gohttp       | https://github.com/codeskyblue/gohttp    | gohttp是一个http的文件服务器，功能有：各种文件的预览功能，实时的目录zip打包下载，二维码扫描下载的支持，苹果应用的在线安装，文件上传等 |
| 13   | API-front    | https://github.com/hidu/api-front        | API front是 HTTP API 前端，可进行请求代理转发、协议抓包分析、流量复制。主要是用于开发测试环境,用来解决开发测试环境多变等问题 |
|    14   |  esumable file uploads |  https://github.com/tus  |  实现文件上传的断点续传功能， 整套功能包含了协议实现，client， server。 client及server有多种语言的实现包括go， python， node等｜
|15  |  pproxy |   https://github.com/hidu/pproxy  |http抓包代理程序,http协议调试工具 |
|   16  |  hystrix-go |    https://github.com/afex/hystrix-go   |    用来隔离远程系统调用， 第三方库调用 ，服务调用， 提供熔断机制，避免雪崩效应的库， Hystrix的go 版本。 注Hystrixs是Netflix开源的一个java库    |

# Web框架
| 序号   | 名称      | 项目地址                                   | 简介                                       |
| ---- | ------- | -------------------------------------- | ---------------------------------------- |
| 1    | Iris-Go | https://github.com/kataras/iris        | 通过Iris-Go，可以方便的帮助你来开发基于web的应用。简单来说：Iris-Go与国内大牛的BeeGo类似，但从其官方介绍的资料来看，Iris-Go的性能更优！ |
| 2    | Baa     | https://github.com/go-baa/baa          | Baa 一个简单高效的Go web开发框架。主要有路由、中间件，依赖注入和HTTP上下文构成。 |
| 3    | Orivil  | https://github.com/orivil/orivil       | Orivil 是由 golang 开发的全新 web 框架，灵感来源于 Laravel 及 Symfony。 |
| 4    | ecgo    | https://github.com/tim1020/ecgo        | ecgo 是一个易学、易用、易扩展的go web开发框架             |
| 5    | Gin     | https://github.com/gin-gonic/gin       | Gin 是一个用 Go 语言开发的 Web 框架，提供类 Martini 的 API，但是性能更好。因为有了 httprouter 性能提升了 40 倍之多。 |
| 6    | Melody  | https://github.com/olahol/melody       | Melody 是一个 Go 语言的微型 WebSocket 框架，基于 github.com/gorilla/websocket 开发， |
| 7    | utron   | https://github.com/gernest/utron       | utron 是一个 Go 语言轻量级的 MVC 框架，用于快速构建可伸缩以及可靠的数据库驱动的 Web 应用。 |
| 8    | Lessgo  | https://github.com/lessgo/lessgo       | Lessgo 是一款 Go 语言编写的简单、稳定、高效、灵活的 web 完全开发框架。它的项目组织形式经过精心设计，实现前后端分离、系统与业务分离，完美兼容MVC与MVVC等多种开发模式，非常利于企业级应用与API接口的开发。当然，最值得关注的是它突破性地支持了运行时路由重建，开发者可在Admin后台轻松实现启用/禁用模块与操作，添加/移除中间件等功能！同时，它推荐以HandlerFunc与MiddlewareFunc为基础的函数式编程，也令开发变得更加灵活富有趣味性。 |
| 9    | Hopen   | https://github.com/who246/hopen        | Golang web极速开发框架。                        |
| 10   | ThinkGo | https://github.com/henrylee2cn/thinkgo | ThinkGo 是一款 Go 语言编写的 web 快速开发框架。它基于开源框架 Echo 进行二次开发，旨在实现一种类 ThinkPHP 的高可用、高效率的 web 框架。在此感谢 Echo 和 httprouter。它最显著的特点是模块、控制器、操作三段式的标准 MVC 架构，且模块与插件的目录结构完全一致，令开发变得非常简单灵活。 |
| 11   | beego   | https://github.com/astaxie/beego       | beego是一个用Go开发的应用框架，思路来自于tornado，路由设计来源于sinatra， |
| 12   | Revel   | https://github.com/robfig/revel        | Revel 是 Go 语言的框架，其思路完全来自 Java 的 Play Framework。 |
| 13   | Martini | https://github.com/codegangsta/martini | Martini 是一个非常新的 Go 语言的 Web 框架，使用 Go 的 net/http 接口开发，类似 Sinatra 或者 Flask 之类的框架，你可使用自己的 DB 层、会话管理和模板。 |
| 14   | Tango   | https://github.com/lunny/tango         | Tango，微内核可扩展的Go语言Web框架。同时支持函数和结构体作为执行体，插件丰富。 |
| 15   | Macaron | https://github.com/go-macaron/macaron  | Macaron 是一个具有高生产力和模块化设计的 Go Web 框架。框架秉承了 Martini 的基本思想，并在此基础上做出高级扩展。 |
| 16   | Web.go  | https://github.com/hoisie/web          | web.go 跟 web.py 类似，但使用的是 Go 编程语言实现的 Web 应用开发框架。Go发布没多久该框架就诞生了，差不多是最早的Go框架。目前已经有段时间没有更新了。不过，该框架代码不多，其源码可以读一读。 |
| 17   | Echo    | https://github.com/labstack/echo       | Echo 是个快速的 HTTP 路由器（零动态内存分配），也是 Go 的微型 Web 框架。 |

# 区块链技术
| 序号   | 名称          | 项目地址                                    | 简介                                       |
| ---- | ----------- | --------------------------------------- | ---------------------------------------- |
| 1    | fabric      | https://github.com/hyperledger/fabric   | Fabric是一个开源区块链实现，开发环境建立在VirtualBox虚拟机上，部署环境可以自建网络，也可以直接部署在BlueMix上，部署方式可传统可docker化，共识达成算法插件化，支持用Go和JavaScript开发智能合约，尤以企业级的安全机制和membership机制为特色。你要是不知道这些术语什么意思，就记住一点，Fabric之于区块链，很可能正如Hadoop之于大数据。 |
| 2    | go-ethereum | https://github.com/ethereum/go-ethereum | go-ethereum客户端通常被称为geth，它是个命令行界面，执行在Go上实现的完整以太坊节点。通过安装和运行geth，可以参与到以太坊前台实时网络并进行以下操作：a. 挖掘真的以太币  b. 在不同地址间转移资金 c .创建合约，发送交易  d . 探索区块历史 e.很多其他功能 |
| 3    | chain       | https://github.com/chain/chain          | **金融领域的区块链项目 **. Chain是由一家刚成立两年的美国创业公司Chain推出，是一个企业级的区块链平台架构，可以让机构构造从零开始更好的金融服务。Chain 开放标准在以下方面实现突破：• 全新的共识模型在不到一秒的时间里实现交易的最终完成，即便是交易量非常大也能支持;• 私密解决方案对区块链数据进行加密，并让相关对手方和监管者进行有选择的读取;• 智能合约框架和虚拟机支持简单的规则执行，以及进行键值存储的图灵完整程序; • 可伸缩的数据模型可以为网络参与者降低运行负荷; • 丰富的元数据层可支持满足KYC（了解你的客户）和 AML（反洗钱）要求 |

# 其它
| 序号   | 名称            | 项目地址                                     | 简介                                       |
| ---- | ------------- | ---------------------------------------- | ---------------------------------------- |
| 1    | kone          | https://github.com/xjdrew/kone           | 可用于家庭或者企业网络的透明代理，可用来翻墙等                  |
| 2    | KodeRunr      | https://github.com/jaxi/koderunr         | KodeRunr (读作 code runner) 是款我在闲暇时间用Go语言编写的应用。顾名思义，你可以用它在网页上、命令行里写程序，贴代码，与此同时无需在本地安装任何编程语言。支持Ruby, Python, GO, Swift, C, Elixir等 |
| 3    | godaemon      | https://github.com/tim1020/godaemon      | godaemon是用来为应用增加daemon和graceful的。        |
| 4    | Gomobile      | https://github.com/golang/mobile         | Gomobile是一个应用于iOS和Android的优秀跨平台开发库，为开发者提供用于创建Android和iOS 移动平台代码的工具。 |
| 5    | gojieba       | https://github.com/yanyiwu/gojieba       | "结巴"中文分词的Golang语言版本。                     |
| 6    | Cherry        | https://github.com/rafael-santiago/cherry | Cherry 是一个使用 Go 语言开发的 Web 聊天引擎。          |
| 7    | MailSlurper   | https://github.com/mailslurper/mailslurper | MailSlurper 是一个便携的 SMTP 邮件服务器，对本地和团队应用开发来说非常有用。MailSlurper 体积小运行快速，支持 SQLite, MSSQL 和 MySQL. 数据库。 |
| 8    | RobustIRC     | https://github.com/robustirc/robustirc   | RobustIRC 是不会有网络中断情况的 IRC。RobustIRC 主要特性：服务器不可用的时候不会有网络中断； 可以使用标准 IRC 客户端； 健壮，可以很好处理客户端和网络的连接问题 |
| 9    | Qor           | https://github.com/qor/qor               | Qor 是基于 Golang 开发的的CMS 一系列工具库，基于 Qor可以快速搭建网站的后台管理系统。Qor 的工作库包含：1，后台管理：可以对数据库进去 CURD 管理，支持一对一，一对多，多对多关联关系维护等等； 2，支持上传图片到云以及 filesystem，resize、crop 图片等等 ；3，Publish 发布系统，可以修改数据，并且经过检查后，再发布到正式环境中； 4，状态机，可以用于开发工作流的系统； 5，I18n，翻译，可以通过在 WEB 界面翻译，并将翻译保存到数据库中； 6，L10n，本地化，不同于翻译，他可以针对某个地区来对内容，或者数据结构进行本地化。7，Roles，权限管理； 8，Exchange，通过 Excel，CSV 导入导出数据； 9，Worker，后台任务管理，可用于跑定时任务等等 |
| 10   | FishChat      | https://github.com/oikomi/FishChatServer | FishChat（鱼传——鱼传尺素）分布式可伸缩 IM 服务器，是一款纯 golang 编写优秀的即时通讯软件(IM), 它集合了市面上已有产品的优点, 并具备 智能硬件网关管理(学习QQ物联思想, 构思中)。 |
| 11   | goRBAC        | https://github.com/mikespook/gorbac      | goRBAC 为 Go 语言应用提供了轻量级的基于角色的访问控制。        |
| 12   | hey           | https://github.com/rakyll/hey            | Boom 是 google 一女工程师使用 Go 语言开发的类似 apache ab 的性能测试工具。相比 ab，boom跨平台性更好，而且更容易安装。 |
| 13   | Mattermost    | https://github.com/mattermost/platform   | mattermost 是一个 Slack 的开源替代品。Mattermost 采用 Go 语言开发，这是一个开源的团队通讯服务。为团队带来跨 PC 和移动设备的消息、文件分享，提供归档和搜索功能。 |
| 14   | glot          | https://github.com/prasmussen/glot       | glot 是可以可以在线运行各种编程语言代码片段的平台，项目采用 Haskell Script 、Go、Erlang 和 Shell 开发，运行环境基于 Docker 容器进行。 |
| 15   | Lantern       | https://github.com/getlantern/lantern    | Lantern是一个点对点科学上网软件。                     |
| 16   | dog-tunnel    | https://github.com/vzex/dog-tunnel       | 狗洞是一个高速的 P2P 端口映射工具，同时支持Socks5代理。 0.5版后开始开源，UDP底层基于开源库KCP重写，效率大大提高，在恶劣环境下优势明显。 同时提供非P2P版本（Lite版本），两端连接过程完全不依赖中间服务器，支持加密和登陆认证，自动重连，但是需要人为确保两端能正常连通（否则请使用默认的P2P版本） |
| 17   | GRPC          | https://github.com/grpc                  | GRPC 是一个高性能、开源和通用的 RPC 框架，面向移动和 HTTP/2 设计。目前提供 C、Java 和 Go 语言版本，分别是：grpc, grpc-java, grpc-go. 其中 C 版本支持 C, C++, Node.js, Python, Ruby, Objective-C, PHP 和 C# 支持.GRPC 基于 HTTP/2 标准设计，带来诸如双向流、流控、头部压缩、单 TCP 连接上的多复用请求等特。这些特性使得其在移动设备上表现更好，更省电和节省空间占用。 |
| 18   | LiteIDE       | https://github.com/visualfc/liteide      | LiteIDE是一款开源、跨平台的轻量级Go语言集成开发环境（IDE）。     |
| 19   | firefly-proxy | https://github.com/yinghuocho/firefly-proxy | 穿墙工具。 GFW梯子。 提供客户端和服务端。支持多个平台， 包括linux， macos， windows ，android |
| 20   | wu            | https://github.com/shanzi/wu/            | 一个监听文件变化并自动执行某些操作的小工具 ，可以用于配置修改后自动重启web server |
| 21   | apex          | https://github.com/apex/apex             | 管理，部署aws lambda函数的工具， 支持用go语言编写lambda函数（注：目前aws官方不支持用go语言编写lambda函数，但是apex却可以变相支持） |
| 22   | gosuv         | https://github.com/codeskyblue/gosuv     | 进程管理， 类似于python的supervisord ， 提供了web管理界面 |

**[⬆ 返回顶部](#目录)**
