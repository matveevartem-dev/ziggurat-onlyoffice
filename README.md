1. ### Выполнить
```cp .env.example .env```

2. ### Выполнить 
- ```hostname -I | awk '{print $1}'```  

- пример вывода
```
$ hostname -I | awk '{print $1}'
192.168.1.10
```

3. #### Отредактировать .env

В ***.env*** файле IP адрес, полученный в п.2, установить как значение для **LOCAL_INTERFACE_IP**

```LOCAL_INTERFACE_IP=192.168.1.10```

4. #### Выполнить
```docker compose up --build -d```
