# Учебные материалы для подготовки к SRE интервью

> 📚 [Навигация по материалам](../NAVIGATION.md)
> 
> 📝 [Вопросы для самопроверки](../self_check/self_check.md)
> ✍️ [Ответы на вопросы](../self_check/answers.md)
> 📖 [Глоссарий](../glossary/glossary.md)

## Содержание
1. [Linux](#linux)
2. [Сетевые технологии](#сетевые-технологии)
3. [Контейнеризация](#контейнеризация)
4. [Kubernetes](#kubernetes)
5. [Мониторинг](#мониторинг)
6. [CI/CD](#cicd)
7. [Базы данных](#базы-данных)
8. [Системный дизайн](#системный-дизайн)
9. [Безопасность](#безопасность)
10. [Автоматизация](#автоматизация)
11. [Отказоустойчивость](#отказоустойчивость)

## Linux

### Основы Linux
1. [Linux для начинающих](https://www.youtube.com/watch?v=sWbUDq4S6Y8) - полный курс на русском
2. [Основы Linux](https://habr.com/ru/company/ruvds/blog/327754/) - статья на Хабре
3. [Linux Command Line](https://www.udemy.com/course/linux-command-line-basics/) - курс на Udemy

### Процесс загрузки
1. [Процесс загрузки Linux](https://habr.com/ru/post/195688/) - подробная статья
2. [Boot Process](https://www.youtube.com/watch?v=XpFsMB6FoOs) - видео на английском

### Файловые системы
1. [Файловые системы Linux](https://habr.com/ru/company/ruvds/blog/327754/) - статья
2. [Inodes в Linux](https://habr.com/ru/post/337350/) - статья

### Ядро Linux
1. [Введение в ядро Linux](https://habr.com/ru/post/195688/) - статья
2. [Linux Kernel](https://www.udemy.com/course/linux-kernel/) - курс на Udemy

## Сетевые технологии

### Основы сетевых протоколов
1. [Сетевые протоколы](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист лекций
2. [TCP/IP](https://habr.com/ru/post/326574/) - статья

### Load Balancing
1. [Load Balancing](https://habr.com/ru/company/ruvds/blog/327754/) - статья
2. [Nginx Load Balancing](https://www.nginx.com/resources/glossary/load-balancing/) - документация

### DNS
1. [DNS](https://habr.com/ru/post/327754/) - статья
2. [DNS Explained](https://www.youtube.com/watch?v=72snZctFFtA) - видео

## Контейнеризация

### Docker
1. [Docker для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья
2. [Docker Tutorial](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

### Docker Compose
1. [Docker Compose](https://docs.docker.com/compose/) - официальная документация
2. [Docker Compose Tutorial](https://www.youtube.com/watch?v=HG6KkjKrG7o) - видео

## Kubernetes

### Основы
1. [Kubernetes для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья
2. [Kubernetes Tutorial](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

### Архитектура
1. [Kubernetes Architecture](https://kubernetes.io/docs/concepts/overview/) - документация
2. [Kubernetes Components](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео

## Мониторинг

### Prometheus
1. [Prometheus Tutorial](https://prometheus.io/docs/introduction/first_steps/) - документация
2. [Prometheus для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Grafana
1. [Grafana Tutorial](https://grafana.com/docs/grafana/latest/getting-started/) - документация
2. [Grafana Dashboard](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео

## CI/CD

### Git
1. [Git Tutorial](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист
2. [Git для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Jenkins
1. [Jenkins Tutorial](https://www.jenkins.io/doc/tutorials/) - документация
2. [Jenkins Pipeline](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео

## Базы данных

### SQL
1. [SQL Tutorial](https://www.w3schools.com/sql/) - учебник
2. [SQL для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### NoSQL
1. [NoSQL Databases](https://www.mongodb.com/nosql-explained) - документация
2. [MongoDB Tutorial](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

### ACID и транзакции
1. [ACID Properties](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео
2. [ACID vs BASE](https://habr.com/ru/company/ruvds/blog/327754/) - статья
3. [Database Transactions](https://www.udemy.com/course/database-transactions/) - курс
4. [ACID Compliance](https://www.databricks.com/blog/2020/10/22/demystifying-acid-compliant-databases.html) - статья
5. [Transaction Isolation Levels](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Репликация и консистентность
1. [Database Replication](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист
2. [Consistency Models](https://habr.com/ru/company/ruvds/blog/327754/) - статья
3. [CAP Theorem](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео
4. [Eventual Consistency](https://www.allthingsdistributed.com/2008/12/eventually_consistent.html) - статья

## Системный дизайн

### Архитектурные паттерны
1. [System Design Primer](https://github.com/donnemartin/system-design-primer) - GitHub репозиторий
2. [System Design Interview](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

### Масштабирование
1. [Scaling Systems](https://habr.com/ru/company/ruvds/blog/327754/) - статья
2. [High Scalability](http://highscalability.com/) - блог

## Практические задания

### Настройка мониторинга
1. [Prometheus + Grafana Tutorial](https://www.youtube.com/watch?v=7bA0gTroJjw) - видео
2. [Monitoring Stack](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Kubernetes Deployment
1. [Kubernetes Hands-on](https://www.udemy.com/course/kubernetes-hands-on/) - курс
2. [Kubernetes Practice](https://github.com/donnemartin/system-design-primer) - GitHub репозиторий

## Дополнительные ресурсы

### Книги
1. [Site Reliability Engineering](https://sre.google/sre-book/table-of-contents/) - Google SRE Handbook
2. [The Practice of System and Network Administration](https://www.amazon.com/Practice-System-Network-Administration-3rd/dp/0321492668) - книга

### Курсы
1. [SRE Course](https://www.coursera.org/learn/site-reliability-engineering-sre) - Coursera
2. [DevOps Course](https://www.udemy.com/course/devops-course/) - Udemy

### Блоги
1. [Google SRE Blog](https://sre.google/blog/) - блог Google SRE
2. [Netflix Tech Blog](https://netflixtechblog.com/) - блог Netflix

## Рекомендации по изучению

1. Начните с базовых тем (Linux, сети)
2. Переходите к контейнеризации и Kubernetes
3. Изучите мониторинг и CI/CD
4. Разберитесь с базами данных
5. Изучите системный дизайн
6. Практикуйтесь на реальных задачах
7. Регулярно повторяйте материал
8. Делайте заметки
9. Решайте практические задания
10. Участвуйте в open-source проектах

## Безопасность

### Основы информационной безопасности
1. [Security Fundamentals](https://www.udemy.com/course/security-fundamentals/) - курс на Udemy
2. [Security Best Practices](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Безопасность контейнеров
1. [Container Security](https://www.docker.com/security) - документация Docker
2. [Kubernetes Security](https://kubernetes.io/docs/concepts/security/) - документация Kubernetes

### Управление секретами
1. [HashiCorp Vault](https://www.vaultproject.io/docs) - документация
2. [Secrets Management](https://habr.com/ru/company/ruvds/blog/327754/) - статья

## Автоматизация

### Ansible
1. [Ansible Tutorial](https://www.ansible.com/resources/get-started) - документация
2. [Ansible для начинающих](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### Terraform
1. [Terraform Tutorial](https://learn.hashicorp.com/terraform) - документация
2. [Infrastructure as Code](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

### Python для автоматизации
1. [Python для DevOps](https://www.udemy.com/course/python-for-devops/) - курс
2. [Python Scripting](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист

## Отказоустойчивость

### Disaster Recovery
1. [DR Planning](https://www.udemy.com/course/disaster-recovery/) - курс
2. [Backup Strategies](https://habr.com/ru/company/ruvds/blog/327754/) - статья

### High Availability
1. [HA Architecture](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист
2. [Load Balancing](https://www.nginx.com/resources/glossary/load-balancing/) - документация

## Производительность

### Профилирование
1. [Performance Profiling](https://www.udemy.com/course/performance-profiling/) - курс
2. [Linux Performance](https://www.brendangregg.com/linuxperf.html) - блог

### Load Testing
1. [JMeter Tutorial](https://www.udemy.com/course/jmeter-tutorial/) - курс
2. [Load Testing Tools](https://habr.com/ru/company/ruvds/blog/327754/) - статья

## Метрики и надежность

### SLO/SLA/SLI
1. [Google SRE: Implementing SLOs](https://sre.google/workbook/implementing-slos/) - официальная документация
2. [SLO/SLA/SLI Explained](https://habr.com/ru/company/ruvds/blog/327754/) - статья на русском
3. [SRE Metrics](https://www.youtube.com/playlist?list=PLSIUOFhnxEiC3YTdxwqZqgEY5imVL8U8J) - плейлист
4. [Error Budgets](https://sre.google/sre-book/implementing-slos/) - документация
5. [SLO Best Practices](https://www.datadoghq.com/blog/slo-monitoring-tracking/) - статья

### Метрики надежности
1. [Reliability Metrics](https://sre.google/sre-book/measuring-slo/) - документация
2. [MTTR/MTBF](https://habr.com/ru/company/ruvds/blog/327754/) - статья
3. [Incident Metrics](https://www.pagerduty.com/blog/incident-metrics/) - статья
4. [Service Level Indicators](https://www.datadoghq.com/blog/service-level-indicators/) - статья

## Типичные вопросы на собеседовании

### Технические вопросы
1. [SRE Interview Questions](https://github.com/michael-kehoe/sre-interview) - GitHub репозиторий
2. [System Design Questions](https://github.com/donnemartin/system-design-primer) - GitHub репозиторий

### Ситуационные задачи
1. [Incident Response](https://response.pagerduty.com) - документация
2. [Postmortems](https://postmortems.pagerduty.com) - документация

### Вопросы о мотивации
1. [SRE Career Path](https://sre.google/sre-book/table-of-contents/) - Google SRE Handbook
2. [SRE Interview Guide](https://www.udemy.com/course/sre-interview/) - курс

## Рекомендации по подготовке к собеседованию

1. Подготовьте рассказ о своем опыте
2. Решите несколько практических задач
3. Изучите типичные вопросы
4. Подготовьте вопросы к интервьюеру
5. Изучите компанию и её технологии
6. Практикуйте решение ситуационных задач
7. Подготовьте портфолио проектов
8. Изучите лучшие практики SRE
9. Подготовьте примеры из реального опыта
10. Изучите метрики и SLO 