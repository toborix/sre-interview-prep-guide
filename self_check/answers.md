# Ответы на вопросы самопроверки SRE

## Linux

### 1. Что такое процесс в Linux?
Процесс в Linux - это экземпляр выполняющейся программы. Каждый процесс имеет:
- Уникальный идентификатор (PID)
- Собственное адресное пространство
- Стек и кучу
- Открытые файловые дескрипторы
- Свойства безопасности

### 2. Как работает виртуальная память?
Виртуальная память в Linux:
- Разделяет физическую память на страницы
- Использует таблицы страниц для отображения
- Поддерживает подкачку (swapping)
- Обеспечивает изоляцию процессов
- Позволяет использовать больше памяти, чем физически доступно

### 3. Что такое inode?
Inode - это структура данных в файловой системе Linux, которая содержит:
- Метаданные файла
- Размер файла
- Права доступа
- Временные метки
- Указатели на блоки данных
- НЕ содержит имя файла

### 4. Как работает процесс загрузки Linux?
1. BIOS/UEFI загружает загрузчик
2. Загрузчик (GRUB) загружает ядро
3. Ядро инициализирует оборудование
4. Запускается systemd (init)
5. Монтируются файловые системы
6. Запускаются сервисы
7. Загружается графический интерфейс (если есть)

### 5. Что такое swap и когда его использовать?
Swap - это файл или раздел на диске, используемый как виртуальная память:
- Используется при нехватке RAM
- Помогает избежать OOM (Out of Memory)
- Может использоваться для гибернации
- Рекомендуется иметь размер 1.5-2x от RAM

## Сетевые технологии

### 1. Как работает TCP/IP?
TCP/IP - стек протоколов:
- IP обеспечивает маршрутизацию пакетов
- TCP обеспечивает надежную передачу
- Использует порты для идентификации сервисов
- Поддерживает установление соединения
- Обеспечивает контроль потока

### 2. Что такое DNS и как он работает?
DNS - система доменных имен:
- Преобразует доменные имена в IP-адреса
- Имеет иерархическую структуру
- Использует кэширование
- Поддерживает различные типы записей
- Обеспечивает отказоустойчивость

### 3. Объясните принцип работы Load Balancing
Load Balancing:
- Распределяет нагрузку между серверами
- Поддерживает различные алгоритмы
- Обеспечивает отказоустойчивость
- Может быть аппаратным или программным
- Поддерживает SSL termination

### 4. Что такое SSL/TLS?
SSL/TLS - протоколы шифрования:
- Обеспечивают безопасную передачу данных
- Используют асимметричное шифрование
- Поддерживают сертификаты
- Обеспечивают аутентификацию
- Защищают от MITM атак

### 5. Как работает HTTP/HTTPS?
HTTP/HTTPS:
- HTTP - протокол передачи данных
- HTTPS - HTTP поверх SSL/TLS
- Использует клиент-серверную модель
- Поддерживает различные методы
- Имеет заголовки и тело запроса

## Контейнеризация

### 1. Что такое Docker и как он работает?
Docker:
- Платформа контейнеризации
- Использует cgroups и namespaces
- Создает изолированные окружения
- Использует слоистую файловую систему
- Поддерживает образы и контейнеры

### 2. В чем разница между контейнером и виртуальной машиной?
Основные различия:
- Контейнеры используют ядро хоста
- ВМ имеют свое ядро
- Контейнеры легче и быстрее
- ВМ обеспечивают лучшую изоляцию
- Контейнеры используют меньше ресурсов

### 3. Как работает Docker Compose?
Docker Compose:
- Управляет множеством контейнеров
- Использует YAML для конфигурации
- Определяет зависимости
- Упрощает развертывание
- Поддерживает переменные окружения

### 4. Что такое Docker Swarm?
Docker Swarm:
- Оркестратор контейнеров
- Обеспечивает кластеризацию
- Поддерживает балансировку
- Управляет репликацией
- Обеспечивает отказоустойчивость

### 5. Как обеспечить безопасность контейнеров?
Меры безопасности:
- Использование официальных образов
- Сканирование уязвимостей
- Ограничение прав
- Обновление базовых образов
- Мониторинг контейнеров

## Kubernetes

### 1. Что такое Pod в Kubernetes?
Pod:
- Минимальная единица развертывания
- Содержит один или несколько контейнеров
- Имеет общее сетевое пространство
- Делит хранилище
- Имеет единый IP-адрес

### 2. Как работает Service в Kubernetes?
Service:
- Обеспечивает доступ к подам
- Поддерживает балансировку
- Имеет различные типы
- Использует селекторы
- Обеспечивает стабильный доступ

### 3. Что такое Deployment и ReplicaSet?
Deployment:
- Управляет репликацией подов
- Обеспечивает обновление
- Поддерживает откат
- Управляет масштабированием
- Использует ReplicaSet

### 4. Как работает ConfigMap и Secret?
ConfigMap:
- Хранит конфигурацию
- Может быть изменен
- Доступен в подах
- Не хранит секреты
- Поддерживает обновление

Secret:
- Хранит секретные данные
- Шифруется в покое
- Безопасное хранение
- Доступен в подах
- Не может быть изменен

### 5. Что такое Ingress?
Ingress:
- Управляет входящим трафиком
- Обеспечивает маршрутизацию
- Поддерживает SSL
- Работает на уровне 7
- Требует Ingress Controller

## Мониторинг

### 1. Что такое SLO/SLA/SLI?
- SLO: целевой уровень обслуживания
- SLA: соглашение об уровне обслуживания
- SLI: индикатор уровня обслуживания
- Все связаны с надежностью сервиса
- Используются для мониторинга

### 2. Как работает Prometheus?
Prometheus:
- Собирает метрики
- Хранит временные ряды
- Поддерживает запросы
- Имеет систему алертинга
- Использует pull-модель

### 3. Какие метрики важны для мониторинга?
Ключевые метрики:
- Latency
- Error rate
- Throughput
- Resource usage
- Business metrics

### 4. Как настроить алерты?
Настройка алертов:
- Определение условий
- Настройка порогов
- Настройка уведомлений
- Тестирование
- Мониторинг ложных срабатываний

### 5. Что такое Error Budget?
Error Budget:
- Допустимое количество ошибок
- Используется для SLO
- Помогает в принятии решений
- Связан с надежностью
- Используется для планирования

## CI/CD

### 1. Что такое CI/CD?
CI/CD:
- Continuous Integration
- Continuous Delivery
- Автоматизация процессов
- Ускорение разработки
- Улучшение качества

### 2. Как работает Git Flow?
Git Flow:
- Ветка master
- Ветка develop
- Feature branches
- Release branches
- Hotfix branches

### 3. Что такое Jenkins Pipeline?
Jenkins Pipeline:
- Автоматизация сборки
- Автоматизация тестирования
- Автоматизация деплоя
- Поддержка различных этапов
- Возможность отката

### 4. Как организовать автоматический деплой?
Автоматический деплой:
- Автоматизация сборки
- Автоматизация тестов
- Автоматизация развертывания
- Мониторинг
- Откат при ошибках

### 5. Что такое Blue/Green deployment?
Blue/Green deployment:
- Два окружения
- Переключение между ними
- Нулевое время простоя
- Возможность отката
- Тестирование в production

## Базы данных

### 1. Что такое ACID?
ACID:
- Atomicity (атомарность)
- Consistency (согласованность)
- Isolation (изоляция)
- Durability (долговечность)
- Свойства транзакций

### 2. Как работает репликация?
Репликация:
- Копирование данных
- Master-Slave
- Master-Master
- Асинхронная
- Синхронная

### 3. Что такое CAP теорема?
CAP теорема:
- Consistency (согласованность)
- Availability (доступность)
- Partition tolerance (устойчивость к разделению)
- Нельзя иметь все три свойства
- Выбор зависит от требований

### 4. Как оптимизировать запросы?
Оптимизация запросов:
- Индексы
- Партиционирование
- Кэширование
- Оптимизация JOIN
- Анализ планов запросов

### 5. Что такое шардирование?
Шардирование:
- Разделение данных
- Горизонтальное масштабирование
- Распределение нагрузки
- Управление ключами
- Балансировка данных

## Системный дизайн

### 1. Как спроектировать масштабируемую систему?
Масштабируемость:
- Горизонтальное масштабирование
- Балансировка нагрузки
- Кэширование
- Асинхронность
- Микросервисы

### 2. Что такое микросервисная архитектура?
Микросервисы:
- Независимые сервисы
- Слабая связанность
- Собственные базы данных
- API для коммуникации
- Независимое развертывание

### 3. Как обеспечить отказоустойчивость?
Отказоустойчивость:
- Репликация
- Балансировка
- Мониторинг
- Автоматическое восстановление
- Тестирование отказов

### 4. Как организовать кэширование?
Кэширование:
- Уровни кэширования
- Стратегии инвалидации
- Распределенное кэширование
- Мониторинг hit/miss
- Оптимизация производительности

### 5. Как обеспечить консистентность данных?
Консистентность:
- ACID
- Eventual consistency
- Strong consistency
- Репликация
- Синхронизация

## Безопасность

### 1. Как обеспечить безопасность инфраструктуры?
Безопасность:
- Файрволы
- SSL/TLS
- Обновления
- Мониторинг
- Аудит

### 2. Как управлять секретами?
Управление секретами:
- Vault
- Encryption
- Access control
- Rotation
- Audit

### 3. Что такое RBAC?
RBAC:
- Role-Based Access Control
- Роли
- Разрешения
- Пользователи
- Группы

### 4. Как организовать аудит безопасности?
Аудит:
- Логирование
- Мониторинг
- Анализ
- Отчеты
- Исправление

### 5. Как защитить от DDoS атак?
Защита от DDoS:
- Rate limiting
- WAF
- CDN
- Мониторинг
- Реагирование

## Автоматизация

### 1. Как автоматизировать рутинные задачи?
Автоматизация:
- Скрипты
- CI/CD
- Мониторинг
- Алертинг
- Документация

### 2. Как использовать Ansible?
Ansible:
- Playbooks
- Inventory
- Roles
- Templates
- Variables

### 3. Как работать с Terraform?
Terraform:
- Infrastructure as Code
- Providers
- Resources
- State
- Modules

### 4. Как писать скрипты автоматизации?
Скрипты:
- Python
- Bash
- PowerShell
- Best practices
- Документация

### 5. Как организовать автоматическое тестирование?
Автоматическое тестирование:
- Unit tests
- Integration tests
- E2E tests
- CI/CD
- Отчеты

## Отказоустойчивость

### 1. Что такое Disaster Recovery?
Disaster Recovery:
- План восстановления
- Резервное копирование
- Тестирование
- Документация
- Процедуры

### 2. Как организовать High Availability?
High Availability:
- Репликация
- Балансировка
- Мониторинг
- Автоматическое восстановление
- Тестирование

### 3. Что такое RTO/RPO?
- RTO: Recovery Time Objective
- RPO: Recovery Point Objective
- Планирование
- Тестирование
- Мониторинг

### 4. Как организовать бэкапы?
Бэкапы:
- Стратегия
- Расписание
- Тестирование
- Хранение
- Мониторинг

### 5. Как тестировать восстановление?
Тестирование:
- План
- Процедуры
- Документация
- Отчеты
- Улучшения 