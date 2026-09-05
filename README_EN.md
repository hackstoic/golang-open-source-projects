# Golang Open Source Projects

A curated Go open source project catalog for English readers. This refreshed list no longer tries to be exhaustive; it prioritizes projects that are still maintained, have clear community recognition, and are useful for learning or technology selection, with additional coverage for AI Agent projects.

Current version includes **78** projects across **10** topics; the latest maintenance status review was completed on **2026-03-06**.

- [Chinese version](README.md)
- [Category and maintenance policy](docs/category-and-maintenance-policy.md)
- [Removal and migration log](docs/removal-and-migration-log.md)

## What Changed in This Refresh

- Reorganized the old 17 loose categories into 10 topic areas and removed the hard-to-maintain "Other" category.
- Removed archived, abandoned, or long-inactive repositories that now have clearer alternatives.
- Removed duplicate entries so each project appears in the most appropriate category only once.
- Added an AI / Agent category covering LLM application frameworks, MCP, inference runtimes, and vector search.

## Selection Principles

- Prefer projects that could still be confirmed as maintained as of 2026-03-06.
- Archived repositories, missing repositories, and long-inactive projects with better alternatives are removed by default.
- Emphasize learning value and practical engineering selection value instead of keeping many edge projects only for coverage.
- Include each project only once to avoid duplication across categories.

## Category Navigation

| Category | Focus | Projects |
| --- | --- | --- |
| AI / Agent | LLM application frameworks, MCP, model runtimes, and vector capabilities | 8 |
| Cloud Native and Containers | Container runtimes, orchestration, registries, and cluster platforms | 8 |
| Service Governance and Platform Engineering | PaaS, service governance, CI/CD, messaging, and async jobs | 12 |
| Data Storage and Search | Databases, distributed storage, search, and data access ecosystems | 10 |
| Observability | Metrics, dashboards, alerting, and runtime health checks | 6 |
| Networking and Security | Gateways, load balancing, proxies, traffic debugging, and network tools | 7 |
| Web Development and Applications | Web frameworks, server-side components, and realtime interaction | 11 |
| Data Processing and Machine Learning | ML, NLP, crawlers, and data processing | 6 |
| Developer Tools and Core Libraries | Developer productivity, testing, terminal UI, and core libraries | 8 |
| Blockchain | Maintained and highly influential Go blockchain projects | 2 |

## AI / Agent

LLM application frameworks, MCP, model runtimes, and vector capabilities

| Project | Description |
| --- | --- |
| [ollama/ollama](https://github.com/ollama/ollama) | A Go runtime for running, distributing, and managing large language models locally. |
| [tmc/langchaingo](https://github.com/tmc/langchaingo) | An LLM application framework for Go, covering prompts, tool calling, agents, and RAG. |
| [cloudwego/eino](https://github.com/cloudwego/eino) | A Go AI application framework from CloudWeGo focused on component orchestration and production use. |
| [mark3labs/mcp-go](https://github.com/mark3labs/mcp-go) | A practical SDK for building MCP clients and servers in Go. |
| [mudler/LocalAI](https://github.com/mudler/LocalAI) | An OpenAI-compatible local inference server suitable for private deployments. |
| [mudler/LocalAGI](https://github.com/mudler/LocalAGI) | An agent platform for local models with an emphasis on tool calling and autonomous workflows. |
| [weaviate/weaviate](https://github.com/weaviate/weaviate) | A vector database written in Go for RAG, retrieval, and agent memory. |
| [pardnchiu/Agenvoy](https://github.com/pardnchiu/Agenvoy) | An agent platform written in Go with Python/JavaScript tool interfaces, error memory, and automatic correction. |

## Cloud Native and Containers

Container runtimes, orchestration, registries, and cluster platforms

| Project | Description |
| --- | --- |
| [moby/moby](https://github.com/moby/moby) | The upstream project for the Docker engine and a core entry point for studying container runtime implementation. |
| [kubernetes/kubernetes](https://github.com/kubernetes/kubernetes) | The de facto standard container orchestration platform. |
| [goharbor/harbor](https://github.com/goharbor/harbor) | An enterprise OCI registry with access control, auditing, and replication features. |
| [rancher/rancher](https://github.com/rancher/rancher) | A Kubernetes management platform for multi-cluster scenarios. |
| [quay/clair](https://github.com/quay/clair) | A container image vulnerability analysis and scanning service. |
| [moby/swarmkit](https://github.com/moby/swarmkit) | The core orchestration component behind Docker Swarm, useful for studying scheduling and cluster orchestration. |
| [AliyunContainerService/pouch](https://github.com/AliyunContainerService/pouch) | Alibaba's open source container engine focused on stronger isolation and stability. |
| [hashicorp/nomad](https://github.com/hashicorp/nomad) | A lightweight workload orchestrator and a useful alternative path to compare with Kubernetes. |

## Service Governance and Platform Engineering

PaaS, service governance, CI/CD, messaging, and async jobs

| Project | Description |
| --- | --- |
| [tsuru/tsuru](https://github.com/tsuru/tsuru) | A mature open source PaaS for learning application platform abstractions. |
| [goodrain/rainbond](https://github.com/goodrain/rainbond) | An application-centric cloud native platform covering delivery, operations, and microservice governance. |
| [harness/harness](https://github.com/harness/harness) | The current CI/CD and developer platform entry point after Drone became part of the Harness ecosystem. |
| [gravitational/teleport](https://github.com/gravitational/teleport) | A zero-trust remote access and infrastructure access platform. |
| [istio/istio](https://github.com/istio/istio) | A representative service mesh project covering traffic management, security, and observability. |
| [uber/jaeger](https://github.com/uber/jaeger) | A distributed tracing system, useful for understanding tracing together with OpenTelemetry. |
| [go-kit/kit](https://github.com/go-kit/kit) | A Go microservices toolkit emphasizing observability and testability. |
| [goadesign/goa](https://github.com/goadesign/goa) | A design-first framework for developing Go services. |
| [TykTechnologies/tyk](https://github.com/TykTechnologies/tyk) | A mature open source API gateway. |
| [micro/go-micro](https://github.com/micro/go-micro) | A Go microservices framework useful for studying service abstractions and plugin-based extension. |
| [nsqio/nsq](https://github.com/nsqio/nsq) | A classic realtime distributed messaging platform. |
| [RichardKnop/machinery](https://github.com/RichardKnop/machinery) | An async task queue for Go and a useful reference for Celery-like designs. |

## Data Storage and Search

Databases, distributed storage, search, and data access ecosystems

| Project | Description |
| --- | --- |
| [cockroachdb/cockroach](https://github.com/cockroachdb/cockroach) | A distributed SQL database focused on strong consistency and elastic scaling. |
| [vitessio/vitess](https://github.com/vitessio/vitess) | YouTube's open source solution for horizontally scaling MySQL. |
| [pingcap/tidb](https://github.com/pingcap/tidb) | A distributed HTAP database compatible with the MySQL protocol. |
| [influxdata/influxdb](https://github.com/influxdata/influxdb) | A classic time series database project. |
| [dgraph-io/dgraph](https://github.com/dgraph-io/dgraph) | A distributed graph database for relationship-heavy query scenarios. |
| [ipfs/kubo](https://github.com/ipfs/kubo) | The Go implementation of IPFS. |
| [chrislusf/seaweedfs](https://github.com/chrislusf/seaweedfs) | A high-performance distributed file system covering object, file, and block storage. |
| [XiaoMi/Gaea](https://github.com/XiaoMi/Gaea) | Xiaomi's open source MySQL middleware focused on sharding and proxy capabilities. |
| [mediocregopher/radix](https://github.com/mediocregopher/radix) | A cleanly designed Go Redis client. |
| [olivere/elastic](https://github.com/olivere/elastic) | A long-standing and widely used Elasticsearch client in the Go ecosystem. |

## Observability

Metrics, dashboards, alerting, and runtime health checks

| Project | Description |
| --- | --- |
| [grafana/grafana](https://github.com/grafana/grafana) | One of the most common observability visualization platforms. |
| [prometheus/prometheus](https://github.com/prometheus/prometheus) | The de facto standard monitoring and time series metrics system. |
| [influxdata/kapacitor](https://github.com/influxdata/kapacitor) | InfluxData's realtime processing, alerting, and monitoring component. |
| [sourcegraph/checkup](https://github.com/sourcegraph/checkup) | A distributed health-checking tool for probing site and service availability. |
| [rapidloop/rtop](https://github.com/rapidloop/rtop) | A lightweight SSH-based remote server monitoring tool. |
| [kubestellar/console](https://github.com/kubestellar/console) | An AI-powered multi-cluster Kubernetes dashboard with realtime observability and 30+ CNCF project integrations. A CNCF Sandbox project. |

## Networking and Security

Gateways, load balancing, proxies, traffic debugging, and network tools

| Project | Description |
| --- | --- |
| [casdoor/casdoor](https://github.com/casdoor/casdoor) | An identity and access management (IAM) / single sign-on (SSO) service with a web UI, supporting OAuth 2.0, OIDC, SAML, CAS, and LDAP. |
| [traefik/traefik](https://github.com/traefik/traefik) | A widely used cloud native reverse proxy and load balancer. |
| [google/seesaw](https://github.com/google/seesaw) | Google's open source Linux load balancing system. |
| [jpillora/go-tcp-proxy](https://github.com/jpillora/go-tcp-proxy) | A simple implementation that is especially useful for learning TCP proxy fundamentals. |
| [probelabs/goreplay](https://github.com/probelabs/goreplay) | A classic tool for replaying production HTTP traffic into test environments. |
| [hidu/pproxy](https://github.com/hidu/pproxy) | An HTTP capture proxy and debugging tool. |
| [getlantern/lantern](https://github.com/getlantern/lantern) | A long-maintained network proxy project and a reference for cross-platform network client design. |

## Web Development and Applications

Web frameworks, server-side components, and realtime interaction

| Project | Description |
| --- | --- |
| [gin-gonic/gin](https://github.com/gin-gonic/gin) | One of the most common high-performance choices among Go web frameworks. |
| [labstack/echo](https://github.com/labstack/echo) | A mature high-performance web framework with a strong API development experience. |
| [beego/beego](https://github.com/beego/beego) | A long-standing full-featured Go web framework that is still maintained. |
| [revel/revel](https://github.com/revel/revel) | A Go web framework with a more full-stack approach. |
| [kataras/iris](https://github.com/kataras/iris) | A web framework emphasizing performance and a complete ecosystem. |
| [go-macaron/macaron](https://github.com/go-macaron/macaron) | A Go web framework with a clear modular style. |
| [andeya/faygo](https://github.com/andeya/faygo) | A Go web framework for API scenarios, with parameter binding and documentation generation. |
| [olahol/melody](https://github.com/olahol/melody) | A lightweight WebSocket framework based on gorilla/websocket. |
| [valyala/fasthttp](https://github.com/valyala/fasthttp) | A highly representative high-performance HTTP implementation in Go. |
| [tus/tusd](https://github.com/tus/tusd) | A server implementation for resumable file uploads. |
| [mattermost/mattermost](https://github.com/mattermost/mattermost) | A representative large Go web application and a good reference for real-world business system organization. |

## Data Processing and Machine Learning

ML, NLP, crawlers, and data processing

| Project | Description |
| --- | --- |
| [gorgonia/gorgonia](https://github.com/gorgonia/gorgonia) | One of the most representative deep learning and tensor computation projects in the Go ecosystem. |
| [cdipaolo/goml](https://github.com/cdipaolo/goml) | Provides implementations for online learning, clustering, regression, and related algorithms. |
| [sjwhitworth/golearn](https://github.com/sjwhitworth/golearn) | A Go library focused more on traditional machine learning workflows. |
| [andeya/pholcus](https://github.com/andeya/pholcus) | A distributed crawler framework written in Go. |
| [yanyiwu/gojieba](https://github.com/yanyiwu/gojieba) | A Go version of the Jieba Chinese word segmentation library. |
| [chrislusf/gleam](https://github.com/chrislusf/gleam) | A Go-style data processing and distributed computing framework. |

## Developer Tools and Core Libraries

Developer productivity, testing, terminal UI, and core libraries

| Project | Description |
| --- | --- |
| [gohugoio/hugo](https://github.com/gohugoio/hugo) | The most representative Go static site generator. |
| [grpc/grpc-go](https://github.com/grpc/grpc-go) | The official Go implementation of gRPC. |
| [rakyll/hey](https://github.com/rakyll/hey) | A lightweight load testing tool. |
| [visualfc/liteide](https://github.com/visualfc/liteide) | A cross-platform Go IDE. |
| [mailslurper/mailslurper](https://github.com/mailslurper/mailslurper) | A very practical test SMTP server for local development. |
| [gizak/termui](https://github.com/gizak/termui) | A Go UI library for building visual dashboards in the terminal. |
| [golang/mobile](https://github.com/golang/mobile) | The official Go mobile development toolchain. |
| [hound-search/hound](https://github.com/hound-search/hound) | A code search tool suitable for self-hosting. |

## Blockchain

Maintained and highly influential Go blockchain projects

| Project | Description |
| --- | --- |
| [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum) | The official implementation of geth, the Ethereum client. |
| [hyperledger/fabric](https://github.com/hyperledger/fabric) | A representative enterprise permissioned blockchain platform. |

## Maintenance Notes

This catalog has removed duplicate entries, outdated repositories, and the old catch-all "Other" category from the previous README. For future expansion, update [projects.json](projects.json) first, run `go run ./tools/generate_readme.go` to refresh the Chinese README, and then update this English README to keep both versions aligned.
