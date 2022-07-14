# Install plugin and setup

- Open Jenkins webapp / manage jenkins / manage plugin
- Install Prometheus metrics
- Install CloudBees Disk Usage Simple
- Configure System 
- Checking here:
 http://devopsempire.synology.me:8080/prometheus/

 # Install Prometheous on Grafana in Docker 
 
 - Login Grafana server
 - install docker if not installed
 - 
 - make new prometheus.yml and copy content user home dir

        sudo docker run -d -p 9090:9090 -v /home/midguard/prometheus.yml:/etc/prometheus/prometheus.yml prom/prometheus

- testing in browser: http://grafanaip:9090
- cheking parameters status / configuration / 
- go back main site: paslte " jenkins_executor_count_value " execute

# Setup Grafana

- Login to grafana
- Remove top panel
- go to / configuration / Datasource / adddatesource / select prometheus
- name " Prometheus-jenkins "
- url: " http://localhost:9090 "
- acces : server 
- save and test
- download dashboard Jenkins: Performance and Health Overview: 
https://grafana.com/grafana/dashboards/?search=jenkins
- Chek number in bwoser link: 9964
- Grafana click + / import pasle here number / load
- Select database










# References

https://www.youtube.com/watch?v=3H9eNIf9KZs