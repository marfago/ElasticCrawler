# ElasticCrawler
ElasticCrawler is a distributed, high configurable, multithreaded web crawler based on Java, Netty nio client, Elasticsearch and Kibana, 

It can be distributed on multiple servers and provides those features:
- configurable url depth
- configurable parallelism degree
- configurable politeness time
- respectfulness of robots.txt directives
- configurable list of included sources
- configurable list of excluded domains
- date detection
- language detection and language based indexing (based on elastic langugae analyzers)
- monitoring console (based on kibana):
  - dashboars on collecter URLs
  - dashboard on collected pages
  - dashboard on query parameters and url structure (useful to detect anomalies or trap urls)

##Benchmark
ElasticCrawler is able to collect and index 40M pages in 12h on a cluster with 3x16CPUs servers (2 Elastic + 1 crawler)

[Crawler](Crawler.png  "Indexed pages")
