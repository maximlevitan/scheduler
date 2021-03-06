# Запуск/останов `mysql` в `docker` контейнере

В `Linux` можно вызовом заготовленного скрипта:
```
./mysql-start.sh
```

Аналогично для останова:
```
./mysql-stop.sh
```

Описания команд запуска и останова смотрите здесь:
https://docs.docker.com/compose/reference/up/
https://docs.docker.com/compose/reference/down/


# Настройки соединения

В настроящий момент мы все можем использовать на своей рабочей машине общие настройки соединения с БД.
Конфигурация `Docker`-контейнера и настроек приложения должна совпадать.
Текущий конфиг соединения:
- Наименование БД: `gbscheduler`
- Хост и порт соединения: `localhost:13306`
- Логин: `root`
- Пароль `qwerty`

Т.к. `Docker`-контейнер с `MySQL` у каждого свои и не доступен во внешний мир, то опасаться публичных настроек для локального окружения не стоит.
