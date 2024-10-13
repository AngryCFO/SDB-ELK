# Домашнее задание к занятию "ELK" - `Александра Бужор`

---

### Задание 1

Elasticsearch
Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный.

Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch. Где будет виден нестандартный cluster_name.

### Решение:

```
    environment:
      - cluster.name=netology-logging
      - xpack.security.enabled=false
      - discovery.type=single-node
```
![image](https://github.com/user-attachments/assets/f1011b8e-0733-4085-a321-ca9f2611bfa6)
![image](https://github.com/user-attachments/assets/7ad70ee9-260d-4a29-bdd2-fe65c5c78212)

---

### Задание 2

Kibana
Установите и запустите Kibana.

Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty.

### Решение:

```
http://localhost:5601/app/dev_tools#/console
```
![image](https://github.com/user-attachments/assets/eaa74957-2287-4bb5-a955-073adef2105f)

---

### Задание 3

Logstash
Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.

### Решение:

![image](https://github.com/user-attachments/assets/c2cf53b0-dec4-4475-8400-96095d374e4d)

---

### Задание 4

Filebeat.
Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.

### Решение:

![image](https://github.com/user-attachments/assets/0c8c463a-40b8-4210-bad1-7ec492c54385)

---
