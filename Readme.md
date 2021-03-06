## Golang Lib for DevOps
  - metrics
  - monitoring
  - servers
  - global locking / paxos / raft
  - Cloud API clients





## Distributed Computing with Golang
  - https://code.google.com/p/go-wiki/wiki/Courses
    - [15-440: Distributed Systems Syllabus](http://www.cs.cmu.edu/~dga/15-440/F12/syllabus.html) - very-very-very good course!
    - [6.824 Lab 1: Lock Server](http://pdos.csail.mit.edu/6.824/labs/lab-1.html)

    - [Chinese Courses](http://billlangjun.github.io/golang.html)

## Locking Server/PubSub/Service Discovery
  - GNats/Nats:
    - http://www.reddit.com/r/golang/comments/1oqqx7/gnatsd_from_apcera_a_high_performance_nats_server/
    - NATS does not have persistence, or transactions. It is more like a nervous system, and it will protect itself at all costs and does not have SPOFs. It does publish/subscribe, and distributed queues.
    - http://www.quora.com/Cloud-Foundry/Why-does-CloudFoundry-use-NATS-a-specially-written-messaging-system-whereas-OpenStack-uses-AMQP
    AMQP, and implementations like RabbitMQ, are enterprise messaging systems built with things like durability, transactions, and formal queues. NATS was designed and built to be like a dial-tone publish-subscribe service, something that is always on and available. However, NATS does not provide durability or transactions, and its queuing model is interest-based only. It also protects itself, the NATS service, at all costs, so that it can always be available. This forms a great base platform for building scalable and reliable distributed systems, but is probably not a good fit for the typical enterprise application.

  - Serf:
    - http://www.serfdom.io/
    - https://news.ycombinator.com/item?id=6600063


## Distributed Execution
  - [Исполнение SSH-команд на сотнях серверов с помощью Golang - 2014.02](http://habrahabr.ru/post/215111/)


## Why Golang for DevOps?
  - [Go Language for Ops and Site Reliability Engineering](http://talks.golang.org/2013/go-sreops.slide)



This repository is supposed to work with [DirEnv](https://github.com/zimbatm/direnv). It will set the GOPATH to current directory and append the ./bin folder to your PATH variable.


<!-- PROJECTS_LIST_START -->
    *** GENERATED BY https://github.com/mindreframer/techwatcher (ruby _sh/pull golang-devops-stuff) *** 

    abh/geodns:
      DNS server with per-client targeted responses
       269 commits, last change: 2014-06-15 - 15:08, 369 stars, 38 forks

    abhishekkr/goshare:
      Go Share your TimeSeries/NameSpace/KeyVal DataStore (using leveldb) over HTTP /or ZeroMQ
       99 commits, last change: 2014-07-23 - 20:55, 48 stars, 5 forks

    ActiveState/tail:
      Go package for reading from continously updated files (tail -f)
       137 commits, last change: 2014-07-28 - 15:34, 151 stars, 36 forks

    adnaan/hamster:
      A back end as a service based on MongoDB
       45 commits, last change: , 57 stars, 4 forks

    apcera/gnatsd:
      High Performance NATS Server
       329 commits, last change: 2014-08-26 - 20:14, 641 stars, 68 forks

    apcera/nats:
      NATS client for Go
       244 commits, last change: 2014-08-15 - 13:40, 167 stars, 21 forks

    ARolek/lilpinger:
      A small site pinging application with email and SMS notifications written in Golang
       5 commits, last change: 2013-12-04 - 14:54, 19 stars, 4 forks

    benbjohnson/go-raft:
      A Go implementation of the Raft distributed consensus protocol.
       543 commits, last change: 2014-08-23 - 16:39, 1,013 stars, 116 forks

    bitly/google_auth_proxy:
      A reverse proxy that provides authentication using Google OAuth2
       32 commits, last change: 2014-08-07 - 17:21, 290 stars, 48 forks

    bitly/nsq:
      A realtime distributed messaging platform
       1,271 commits, last change: 2014-08-26 - 10:42, 3,191 stars, 297 forks

    bradfitz/runsit:
      It runs it.
       69 commits, last change: 2013-09-24 - 10:45, 192 stars, 16 forks

    buger/cloud-ssh:
      Cloud enhanced SSH client replacement with host auto-completion
       29 commits, last change: 2014-08-20 - 19:22, 33 stars, 3 forks

    buger/gor:
      HTTP traffic replay in real-time. Replay traffic from production to staging and dev environments.
       349 commits, last change: 2014-08-21 - 16:39, 1,610 stars, 84 forks

    BurntSushi/cmail:
      cmail runs a command and sends the output to your email address at certain intervals.
       11 commits, last change: , 3 stars, 0 forks

    calmh/syncthing:
      Open Source Continuous File Synchronization
       967 commits, last change: 2014-08-29 - 12:36, 4,308 stars, 237 forks

    ccding/go-stun:
      a go implementation of the STUN client (RFC 3489 and RFC 5389)
       4 commits, last change: , 19 stars, 2 forks

    cloudflare/redoctober:
      Go server for two-man rule style file encryption and decryption.
       74 commits, last change: 2014-07-08 - 19:35, 718 stars, 53 forks

    cloudfoundry/gorouter:

       468 commits, last change: 2014-08-21 - 21:27, 162 stars, 75 forks

    cloudfoundry/gosigar:

       28 commits, last change: 2014-06-25 - 16:11, 84 stars, 31 forks

    cloudfoundry/hm9000:

       331 commits, last change: 2014-08-20 - 16:16, 25 stars, 14 forks

    cloudfoundry/yagnats:
      Yet Another Go NATS client
       78 commits, last change: 2014-08-07 - 12:33, 7 stars, 2 forks

    coreos/etcd:
      A highly-available key value store for shared configuration and service discovery
       1,985 commits, last change: 2014-08-28 - 14:38, 3,984 stars, 396 forks

    coreos/rudder:
      Rudder is an etcd backed overlay network for containers
       42 commits, last change: 2014-08-28 - 22:36, 58 stars, 3 forks

    crosbymichael/skydock:
      Service discovery via DNS for docker
       91 commits, last change: 2014-07-28 - 11:00, 566 stars, 42 forks

    crowdmob/goamz:
      Fork of the GOAMZ version developed within Canonical with additional functionality with DynamoDB
       724 commits, last change: 2014-08-24 - 16:57, 209 stars, 129 forks

    dotcloud/docker:
      Docker - the open-source application container engine
       10,267 commits, last change: 2014-08-28 - 18:40, 14,678 stars, 2,752 forks

    efficient/epaxos:

       26 commits, last change: 2014-01-20 - 08:21, 187 stars, 9 forks

    erikh/gollector:
      json-based metrics collector
       176 commits, last change: 2014-07-24 - 18:41, 112 stars, 6 forks

    errplane/errplane-go:
      Go library for metrics for Errplane
       52 commits, last change: 2013-08-21 - 17:51, 16 stars, 3 forks

    flynn/go-crypto-ssh:
      Forked from go.crypto as Flynn working copy until changes merged upstream
       9 commits, last change: 2014-06-28 - 20:51, 1 stars, 2 forks

    flynn/go-discover:
      Archived -- see https://github.com/flynn/flynn
       138 commits, last change: 2014-08-02 - 13:58, 238 stars, 24 forks

    flynn/rpcplus:
      Archived -- see https://github.com/flynn/flynn
       38 commits, last change: 2014-08-02 - 13:57, 18 stars, 3 forks

    globocom/gandalf:
      Gandalf is an API to manage git repositories.
       665 commits, last change: 2014-08-28 - 22:17, 138 stars, 23 forks

    globocom/tsuru:
      Open source Platform as a Service (PaaS).
       7,886 commits, last change: 2014-08-27 - 15:44, 1,160 stars, 117 forks

    gogits/gogs:
      Gogs(Go Git Service) is a painless self-hosted Git Service written in Go.
       1,229 commits, last change: 2014-08-24 - 20:42, 3,622 stars, 221 forks

    golang/groupcache:
      groupcache is a caching and cache-filling library, intended as a replacement for memcached in many cases.
       27 commits, last change: 2014-07-09 - 07:38, 2,996 stars, 265 forks

    happypancake/fsd:
      Func based statsd client for golang, which returns more or less directly via using a buffered channel and reconnection establishment in case of failure of udp sending
       23 commits, last change: 2014-03-14 - 05:16, 1 stars, 0 forks

    hashicorp/serf:
      Service orchestration and management tool.
       1,189 commits, last change: 2014-08-28 - 17:31, 2,378 stars, 163 forks

    hashicorp/terraform:
      Terraform is a tool for building, changing, and combining infrastructure safely and efficiently.
       1,487 commits, last change: 2014-08-28 - 17:27, 1,394 stars, 89 forks

    inconshreveable/muxado:
      Stream multiplexing for Go
       15 commits, last change: 2014-03-12 - 01:58, 209 stars, 11 forks

    inconshreveable/ngrok:
      Introspected tunnels to localhost
       295 commits, last change: 2014-08-06 - 08:57, 3,089 stars, 196 forks

    inconshreveable/slt:
      A TLS reverse proxy with SNI multiplexing in Go
       9 commits, last change: , 99 stars, 4 forks

    influxdb/influxdb:
      Scalable datastore for metrics, events, and real-time analytics
       2,345 commits, last change: 2014-08-27 - 11:19, 2,811 stars, 215 forks

    jingweno/gotask:
      Idiomatic build tool in Go
       123 commits, last change: 2014-01-12 - 10:05, 140 stars, 5 forks

    joewalnes/websocketd:
      Turn any program that uses STDIN/STDOUT into a WebSocket server. Like inetd, but for WebSockets.
       154 commits, last change: 2014-07-26 - 21:38, 3,358 stars, 146 forks

    jondot/groundcontrol:
      Manage and monitor your Raspberry Pi with ease
       50 commits, last change: 2013-08-22 - 07:19, 673 stars, 46 forks

    jordansissel/lumberjack:
      An experiment to cut logs in preparation for processing elsewhere.
       560 commits, last change: 2014-08-22 - 05:02, 732 stars, 192 forks

    jyap808/jaeger:
      Jaeger is a JSON encoded GPG encrypted key value store. It is useful for generating and keeping configuration files secure. Jaeger is written in Go.
       38 commits, last change: 2014-05-01 - 14:55, 10 stars, 3 forks

    kelseyhightower/confd:
      Manage local application configuration files using templates and data from etcd or consul
       283 commits, last change: 2014-08-08 - 11:14, 821 stars, 78 forks

    mailgun/vulcan:
      Golang HTTP reverse proxy library
       332 commits, last change: 2014-08-27 - 13:14, 260 stars, 19 forks

    mindreframer/emtail:
      extract whitebox monitoring data from logs and insert into a timeseries database - mirror for https://code.google.com/p/emtail/
       273 commits, last change: , 1 stars, 0 forks

    mitchellh/go-ps:
      Find, list, and inspect processes from Go (golang).
       19 commits, last change: 2014-04-07 - 16:34, 176 stars, 9 forks

    mitchellh/packer:
      Packer is a tool for creating identical machine images for multiple platforms from a single source configuration.
       3,149 commits, last change: 2014-08-26 - 14:06, 2,916 stars, 513 forks

    mozilla-services/heka:
      Data collection and processing made easy.
       2,785 commits, last change: 2014-08-28 - 19:50, 1,518 stars, 151 forks

    mrwilson/helixdns:
      A simple dns server that reads records from etcd.
       54 commits, last change: 2014-08-09 - 11:00, 46 stars, 8 forks

    necrogami/watchdog:
      Watchdog
       7 commits, last change: , 2 stars, 1 forks

    nf/gohttptun:
      A tool to tunnel TCP over HTTP, written in Go
       22 commits, last change: 2014-01-22 - 13:29, 100 stars, 16 forks

    nuxeo/gogeta:
      Reverse proxy based on etcd hierarchy
       76 commits, last change: 2014-08-26 - 14:56, 88 stars, 8 forks

    oleiade/trousseau:
      Networked and encrypted key-value database
       273 commits, last change: 2014-08-14 - 11:19, 609 stars, 23 forks

    petar/GoTeleport:
      Teleport Transport: End-to-end resilience to network outages
       6 commits, last change: , 122 stars, 2 forks

    pubsubsql/pubsubsql:
      An open-source distributed in-memory database integrated with Publish-Subscribe
       452 commits, last change: , 42 stars, 6 forks

    PuerkitoBio/throttled:
      throttling strategies for HTTP handlers
       39 commits, last change: 2014-02-25 - 09:02, 184 stars, 6 forks

    rackspace/gophercloud:
      The Go SDK for Openstack.
       226 commits, last change: 2014-08-15 - 17:33, 220 stars, 33 forks

    rcrowley/go-metrics:
      Go port of Coda Hale's Metrics library
       234 commits, last change: 2014-08-23 - 15:20, 525 stars, 75 forks

    ReshNesh/pixlserv:
      Go server for processing and serving of images
       148 commits, last change: 2014-07-15 - 14:31, 262 stars, 9 forks

    rzab/ostent:
      A drop-in system metrics inspector
       281 commits, last change: 2014-08-26 - 19:46, 21 stars, 1 forks

    Sendhub/shipbuilder:
      The Open-source self-hosted Platform-as-a-Service written in Go
       139 commits, last change: 2014-01-06 - 16:41, 8 stars, 39 forks

    shirkey/go-guerrilla:
      Mini SMTP server written in golang
       28 commits, last change: , 2 stars, 25 forks

    skydb/sky:
      Sky is an open source, behavioral analytics database.
       559 commits, last change: 2014-08-03 - 22:20, 657 stars, 62 forks

    skynetservices/skydns:
      DNS service discovery for etcd
       398 commits, last change: 2014-08-25 - 07:40, 271 stars, 38 forks

    smira/aptly:
      aptly - Debian repository management tool
       846 commits, last change: 2014-08-29 - 00:53, 340 stars, 25 forks

    spf13/nitro:
      Quick and easy performance analyzer library for golang
       7 commits, last change: 2013-10-03 - 09:43, 121 stars, 6 forks

    stripe-ctf/octopus:
      Many-armed network simulator
       17 commits, last change: , 64 stars, 2 forks

    tsenart/tb:
      A generic lock-free implementation of the "Token-Bucket" algorithm
       54 commits, last change: 2014-06-25 - 04:22, 53 stars, 2 forks

    tsenart/vegeta:
      HTTP load testing tool and library. It's over 9000!
       203 commits, last change: 2014-07-01 - 21:47, 1,717 stars, 82 forks

    uniqush/uniqush-push:
      Uniqush is a free and open source software which provides a unified push service for server-side notification to apps on mobile devices.
       415 commits, last change: 2014-06-29 - 18:48, 505 stars, 66 forks

    vektra/tachyon:
      An experimental configuration management system inspired by ansible
       133 commits, last change: 2014-08-25 - 21:23, 73 stars, 11 forks

    vito/garden:
      Go Warden
       287 commits, last change: 2014-02-09 - 13:11, 0 stars, 8 forks

    VividCortex/robustly:
      Run functions resiliently in Go, catching and restarting panics
       33 commits, last change: , 69 stars, 2 forks

    xtaci/gonet:
      a game server skeleton in golang
       4 commits, last change: 2014-08-18 - 12:59, 276 stars, 120 forks

    YuriyNasretdinov/GoSSHa:
      Ssh client that supports multiple servers
       21 commits, last change: 2014-07-15 - 14:40, 49 stars, 7 forks

    zimbatm/socketmaster:
      Zero downtime restarts for your apps
       51 commits, last change: 2014-01-31 - 15:54, 424 stars, 19 forks
<!-- PROJECTS_LIST_END -->
