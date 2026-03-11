# Awesome Gatling [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) with stars

<!--lint ignore double-link match-punctuation -->

[<img src="assets/images/gatling-logo.svg" align="right" width="260" alt="Gatling">](https://gatling.io/)

<!--lint ignore double-link-->

A curated collection of resources covering all aspects of load testing using [Gatling](https://gatling.io/) and related stuff: plugins, integrations, testing techniques, DevOps practices, etc.

<!--lint ignore double-link-->

> [Gatling](https://gatling.io/) is an open-source load and performance testing framework based on Scala, Akka and Netty.

## Contents

* [Official Resources](#official-resources)
* [Getting Started](#getting-started)
* [Tutorials](#tutorials)
* [Distributed Testing](#distributed-testing)
* [Tools](#tools)
  * [Plugins](#plugins)
  * [Frameworks](#frameworks)
  * [Reporting](#reporting)
  * [Sandbox](#sandbox)
  * [Miscellaneous](#miscellaneous)
* [CI](#ci)
* [Test Management](#test-management)
* [Trainings & Courses](#trainings--courses)
* [Videos](#videos)
  * [Talks](#talks)
  * [Video Tutorials](#video-tutorials)
* [Community](#community)
* [Related](#related)
  * [Awesome Lists](#awesome-lists)
  * [Other](#other)

## Official Resources

<!--lint ignore double-link-->

* [Homepage](https://gatling.io/)
* [Documentation](https://docs.gatling.io/)
* [Source code](https://github.com/gatling/gatling) ⭐ 6,872 | 🐛 27 | 🌐 Scala | 📅 2026-03-10

## Getting Started

* [A first look at Gatling, a DSL based load test tool](https://callistaenterprise.se/blogg/teknik/2014/04/16/a-first-look-at-gatling-a-dsl-based-load-test-tool/)
* [Gatling: Take your performance tests to the next level](https://www.thoughtworks.com/insights/blog/gatling-take-your-performance-tests-next-level)
* [Load Testing with Gatling. The Complete Guide](https://www.james-willett.com/gatling-load-testing-complete-guide/)

## Tutorials

* [Load testing gRPC services with Gatling](https://medium.com/@georgeleung_7777/load-testing-grpc-services-with-gatling-990025c77055)
* [Creating a custom Gatling protocol for AWS Lambda](https://callistaenterprise.se/blogg/teknik/2016/11/26/gatling-custom-protocol/)
* [Load testing ZeroMQ with a custom DSL for Gatling](https://mintbeans.com/load-testing-zeromq-with-gatling/)

## Distributed Testing

* [Distributed Gatling](https://github.com/Abiy/distGatling) ⭐ 103 | 🐛 48 | 🌐 CSS | 📅 2023-01-04 - Solution to run Gatling simulation tests in a distributed/cluster environment.
* [gatling-operator](https://github.com/st-tech/gatling-operator) ⭐ 82 | 🐛 17 | 🌐 Go | 📅 2025-09-18 - Automating distributed Gatling load testing using Kubernetes operator.
* [Distributed load testing with Gatling and Kubernetes](https://debijenkorf.tech/https-medium-com-annashepeleva-distributed-load-testing-with-gatling-and-kubernetes-93ebce26edbe)
* [Gatling – Scaling Out Your Load Tests](https://web.archive.org/web/20210625094528/http://www.nimrodstech.com/gatling-cluster-load-testing/)

## Tools

### Plugins

* [gatling-dubbo](https://github.com/youzan/gatling-dubbo) ⭐ 153 | 🐛 4 | 🌐 Scala | 📅 2019-08-20 - A Gatling plugin for running load tests on Apache Dubbo.
* [gatling-grpc](https://github.com/phiSgr/gatling-grpc) ⚠️ Archived - Gatling load test plugin for gRPC.
* [gatling-sbt-plugin](https://github.com/gatling/gatling-sbt-plugin) ⭐ 109 | 🐛 1 | 🌐 Scala | 📅 2026-03-01 - Gatling SBT plugin to integrate Gatling with SBT, allowing to use Gatling as a testing framework.
* [gatling-kafka](https://github.com/mnogu/gatling-kafka) ⚠️ Archived - A Gatling plugin for stress testing Apache Kafka protocol.
* [gatling-mqtt](https://github.com/mnogu/gatling-mqtt) ⚠️ Archived - A Gatling plugin for stress testing MQTT.
* [gatling-maven-plugin](https://github.com/gatling/gatling-maven-plugin) ⭐ 38 | 🐛 1 | 🌐 Java | 📅 2026-03-09 - Gatling Maven Extensions.
* [gatling-gradle-plugin](https://github.com/gatling/gatling-gradle-plugin) ⭐ 30 | 🐛 0 | 🌐 Groovy | 📅 2026-03-05 - Gatling plugin for Gradle.
* [gatling-tcp-extensions](https://github.com/scalecube/gatling-tcp-extensions) ⭐ 23 | 🐛 5 | 🌐 Scala | 📅 2023-04-16 - TCP extensions for Gatling.
* [gatling-kafka](https://github.com/Amerousful/gatling-kafka) ⭐ 18 | 🐛 4 | 🌐 Scala | 📅 2026-01-23 - Gatling plugin for Kafka.
* [gatling-thrift](https://github.com/3tty0n/gatling-thrift) ⚠️ Archived - Gatling third party plugin for Apache Thrift.
* [gatling-kafka-plugin](https://github.com/galax-io/gatling-kafka-plugin) ⭐ 15 | 🐛 15 | 🌐 Scala | 📅 2026-03-08 - Plugin for support Kafka in Gatling.
* [gatling-aws](https://github.com/callistaenterprise/gatling-aws) ⭐ 11 | 🐛 2 | 🌐 Scala | 📅 2018-11-14 - Gatling custom protocol for AWS Lambda.
* [gatling-wait](https://github.com/Amerousful/gatling-wait) ⭐ 11 | 🐛 0 | 🌐 Scala | 📅 2026-02-27 - Plugin that simplifies waiting for specific events allowing customizable conditions, attempt management, and error handling.
* [gatling-remote-sbt](https://github.com/Pravoru/gatling-remote-sbt) ⭐ 10 | 🐛 0 | 🌐 Scala | 📅 2020-04-29 - Remote execution plugin for Gatling load tests.
* [gatling-jdbc-plugin](https://github.com/galax-io/gatling-jdbc-plugin) ⭐ 6 | 🐛 5 | 🌐 Scala | 📅 2026-03-08 - Simple Gatling plugin for JDBC support.
* [gatling-sql](https://github.com/tmcgrath/gatling-sql) ⭐ 6 | 🐛 2 | 🌐 Scala | 📅 2021-04-22 - Gatling extension for JDBC or Spark Thrift Server stress testing.
* [gatling-amqp-plugin](https://github.com/galax-io/gatling-amqp-plugin) ⭐ 5 | 🐛 2 | 🌐 Scala | 📅 2026-03-08 - Plugin for support performance testing with AMQP in Gatling (3.2.x).
* [gatling-zeromq](https://github.com/softwaremill/gatling-zeromq) ⚠️ Archived - A Gatling stress test plugin for ZeroMQ protocol.
* [gatling-xmpp-protocol](https://github.com/TLmaK0/gatling-xmpp-protocol) ⭐ 4 | 🐛 0 | 🌐 Scala | 📅 2018-11-13 - XMPP protocol for stress test XMPP servers with Gatling.
* [gatling-picatinny](https://github.com/galax-io/gatling-picatinny) ⭐ 4 | 🐛 3 | 🌐 Scala | 📅 2026-02-10 - Library with a bunch of useful functions that extend Gatling DSL.
* [gatling-build-plugin](https://github.com/gatling/gatling-build-plugin) ⭐ 3 | 🐛 0 | 🌐 Scala | 📅 2026-03-01 - An SBT plugin to share common settings across Gatling's projects' builds.
* [gatling-junitrunner](https://github.com/Pravoru/gatling-junitrunner) ⭐ 3 | 🐛 1 | 🌐 Scala | 📅 2018-11-09 - JUnit wrapper around Gatling simulations.
* [gatling-bolt](https://github.com/sarmbruster/gatling-bolt) ⭐ 2 | 🐛 5 | 🌐 Scala | 📅 2021-02-16 - Support Neo4j Bolt protocol for Gatling.
* [gatling-jwt](https://bitbucket.org/atlassianlabs/gatling-jwt/) - An extension to Gatling 2.0 to help make JWT-signed requests.

### Frameworks

* [Kraken](https://github.com/OctoPerf/kraken) ⭐ 118 | 🐛 54 | 🌐 Java | 📅 2024-02-15 - Load testing IDE based on Gatling by OctoPerf.
* [Gatlytron](https://github.com/Performetriks/Gatlytron) ⭐ 3 | 🐛 0 | 🌐 Java | 📅 2025-12-04 - Gatling Base Framework for easy onboarding.
* [Karate Gatling](https://karatelabs.github.io/karate/karate-gatling/) - Re-use Karate API-tests as performance tests executed by Gatling.
* [Taurus](https://gettaurus.org/docs/Gatling/) - Gatling Executor in Taurus framework.
* [Carrier](https://github.com/carrier-io) - Continuous test execution platform with ability to perform load testing using customized JMeter and Gatling containers.

### Reporting

* [gatling-report](https://github.com/nuxeo/gatling-report) ⭐ 125 | 🐛 14 | 🌐 Java | 📅 2026-02-17 - Parse Gatling simulation.log files to output CSV stats or build HTML reports with Plotly charts.
* [gatling-elasticsearch](https://github.com/Amerousful/gatling-elasticsearch-logs) ⭐ 16 | 🐛 4 | 🌐 Scala | 📅 2026-03-09 - Logger which parses raw Gatling logs and sends them to the Elasticsearch.
* [gatling2allure](https://github.com/biski/gatling2allure) ⭐ 6 | 🐛 0 | 🌐 Java | 📅 2024-12-10 - Convert Gatling log to Allure report.

### Sandbox

* [gatling-scaffold](https://github.com/robsonbittencourt/gatling-scaffold) ⭐ 17 | 🐛 0 | 🌐 Kotlin | 📅 2025-09-24 - Base for load test project using Gatling, InfluxDB and Grafana.
* [perfiz](https://github.com/znsio/perfiz) ⭐ 15 | 🐛 8 | 🌐 Scala | 📅 2025-12-27 - A dockerised API performance test setup based on Gatling with Grafana dashboards and Prometheus monitoring.

### Miscellaneous

* [dakiya](https://github.com/rupeshmore/dakiya) ⭐ 37 | 🐛 3 | 🌐 JavaScript | 📅 2017-03-07 - Convert Postman collections to Gatling scripts.
* [gatling-template.g8](https://github.com/galax-io/gatling-template.g8) ⭐ 3 | 🐛 1 | 🌐 Scala | 📅 2026-02-10 - A Giter8 template for Gatling performance test project.

## CI

* [Gatling Jenkins Plugin](https://github.com/jenkinsci/gatling-plugin) ⭐ 36 | 🐛 2 | 🌐 Java | 📅 2025-06-16 - [Jenkins plugin](https://plugins.jenkins.io/gatling/) for Gatling.
* [run-gatling](https://github.com/liatrio/run-gatling) ⚠️ Archived - GitHub Action to easily integrate Gatling performance tests to GitHub workflows.

## Test Management

* [Performance and load testing with Gatling](https://docs.getxray.app/space/XRAYCLOUD/44565472/Performance+and+load+testing+with+Gatling) - Integrating with Xray Test Management on Jira and Gatling.

## Trainings & Courses

* [Gatling Courses](https://www.udemy.com/topic/gatling/) - By Udemy.
* [Performance Test Automation 101: Gatling, Lighthouse, & Jenkins](https://www.educative.io/courses/performance-test-automation-101-gatling-lighthouse-jenkins) - By Educative.

## Videos

### Talks

* [Load Testing Done Right with Gatling](https://www.youtube.com/watch?v=VUPTaPms210) - Stéphane Landelle @ Voxxed Days Belgrade 2015.
* [Load Testing Crash Course with Gatling](https://www.youtube.com/watch?v=RiM1GsVSbzM) - Stéphane Landelle @ Devoxx Belgium 2022.
* [Load Testing Made Easy with Gatling](https://www.youtube.com/watch?v=8Eplj8BvugA) - Rafał Piotrowski @ Scala Days 2023 Madrid.

### Video Tutorials

* [Performance Testing with Gatling](https://www.youtube.com/playlist?list=PLd4gvNaNZ4T3NCWsv3zwHYlLGtr9s1-Fz) - Tutorial series by Tomi Tiihonen.
* [Gatling Tutorials for Beginners](https://www.youtube.com/playlist?list=PLw_jGKXm9lIYpTotIJ-R31pXS7qqwXstt) - Tutorial series by James Willett.

## Community

* [Gatling Community](https://community.gatling.io/)
* [`gatling` on Stack Overflow](https://stackoverflow.com/questions/tagged/gatling+or+scala-gatling+or+gatling-java+or+gatling-plugin)
* [`@GatlingTool` on Twitter](https://x.com/gatlingtool)

## Related

### Awesome Lists

* [Awesome Software Quality](https://github.com/ligurio/sqa-wiki) ⭐ 2,311 | 🐛 0 | 📅 2023-02-01 - A list of free software testing and verification resources.
* [Awesome Testing](https://github.com/TheJambo/awesome-testing) ⭐ 2,217 | 🐛 1 | 📅 2026-03-05 - A curated list of testing resources.
* [Awesome JMeter](https://github.com/aliesbelik/awesome-jmeter) ⭐ 776 | 🐛 0 | 🌐 HTML | 📅 2026-03-09 - Open-source load testing and performance measurement tool, written in Java.
* [Awesome k6](https://github.com/grafana/awesome-k6) ⭐ 743 | 🐛 4 | 📅 2026-03-05 - Open-source, developer-centric performance monitoring and load testing solution.
* [Awesome Locust](https://github.com/aliesbelik/awesome-locust) ⭐ 111 | 🐛 0 | 📅 2026-03-10 - Open-source scalable load testing framework written in Python.
* [Awesome Tsung](https://github.com/aliesbelik/awesome-tsung) ⭐ 23 | 🐛 0 | 📅 2026-03-05 - Open-source multi-protocol distributed load testing tool, developed in Erlang.

### Other

* [Load Testing Toolkit](https://github.com/aliesbelik/load-testing-toolkit) ⭐ 234 | 🐛 0 | 📅 2026-02-16 - Collection of open-source tools for debugging, benchmarking, load and stress testing your code or services.
* [How They Load Test](https://github.com/aliesbelik/how-they-load) ⭐ 151 | 🐛 0 | 📅 2025-12-01 - A curated collection of publicly available resources on how companies around the world perform load testing.

## Contributing

Contributions are welcome!<br>
Please take a look at the [CONTRIBUTING](origin/CONTRIBUTING.md) guidelines first.
