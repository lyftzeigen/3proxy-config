# 3proxy-config
Конфигурация для 3proxy в сочетании с контейнером https://github.com/QAutomatron/docker-3proxy

### 1. Для установки контейнера
```bash
docker pull qautomatron/docker-3proxy:latest
```

### 2. Для запуска контейнера с данными настройками
```bash
docker run --name='3proxy' --restart=always -d -v $(pwd)/3proxy.cfg:/etc/3proxy/3proxy:ro -p 8080:8080 qautomatron/docker-3proxy:latest
```

### 3. Добавить пользователя можно в файл конфигурации
```bash
users username:CL:password
```
