#tick-stack & spring boot 2
---

Spring Boot 2

&

Telegraf: collects time-series data from a variety of sources.
InfluxDB: stores time-series data.
Chronograf: visualizes and graphs the time-series data.
Kapacitor: provides alerting and detects anomalies in time-series data.

---

1. Add Maven Dependency

<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-actuator</artifactId>
</dependency>

2. Add Configuration in `application.properties`
management.metrics.export.statsd.enabled=true
management.metrics.export.statsd.flavor=telegraf
management.metrics.export.statsd.port=8125

3. Read docs
https://micrometer.io/docs
https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#production-ready
