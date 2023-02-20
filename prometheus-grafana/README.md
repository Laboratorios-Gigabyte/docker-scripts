# Project Docker to start Prometheus and Grafana


## Steps to start servides

### Step 0

#### We need to enable actutor in youe Spring boot application

Spring boot Actuator
- [Actuator Documentation](https://docs.spring.io/spring-boot/docs/current/actuator-api/htmlsingle/)
- [Enabling actuator](https://www.appsdeveloperblog.com/how-to-enable-actuators-httptrace-in-spring-boot-3/)
  - [Prometheus Endpoint](http://localhost:8080/actuator/prometheus)
  - [Info Endpoint](http://localhost:8080/actuator/info)
  - [Health Endpoint](http://localhost:8080/actuator/prometheus)


### Step 1

- [Sample Spring Boot/Prometheus/Grafana](https://youtu.be/pVdDWQQeqME)

We need to modify [Prometheus Config file](https://github.com/Laboratorios-Gigabyte/docker-scripts/blob/cd13da40679482bce89047edb7c78d1a66a7e667/prometheus-grafana/data/prometheus/config/prometheus.yml#L14) substitute the IP with the IP where your application is deployed.

To start Prometheus and Grafana
```
$>doker-compose up
```


