### Spring Cloud Netflix Eureka Server
Eureka Server - одна из реализаций паттерна [Service Registry](https://jstobigdata.com/architecture/service-discovery-pattern-in-microservices/).
Он позволяет микросервисам динамически регистрироваться и обнаруживать друг друга без необходимости
жесткой кодировки URL или адресов в конфигурациях. Каждый микросервис, запущенный в системе,
может зарегистрироваться в Eureka Server, указав свое имя, адрес (хост и порт) и другие метаданные.
Эта зависимость находится только в сервисе service-discovery. Для подключения к eureka server остальные сервисы
имеют зависимость spring-cloud-starter-netflix-eureka-client