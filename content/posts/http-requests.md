---
title: "HTTP запросы: Telnet, netcat, cURL, Postman"
date: 2026-06-01
draft: false
---

## Задание 1 — GET и POST через Telnet/netcat

### GET через Telnet

```bash
telnet example.com 80
GET / HTTP/1.1
Host: example.com

```

![get](/img/get.jpg)
![post](https://github.com/fkea1da/portfolio/blob/main/static/img/post.jpg?raw=true)   

### GET через netcat

```bash
echo -e "GET /get HTTP/1.1\r\nHost: httpbin.org\r\nConnection: close\r\n\r\n" | nc httpbin.org 80
```

## Задание 2 — cURL

### GET запрос

```bash
curl -X GET "https://api.publicapis.org/entries?category=animals"
```

### POST запрос

```bash
curl -X POST https://httpbin.org/post -H "Content-Type: application/json" -d '{"name": "Ilya", "age": 20}'
```

![curl](..img/curl.jpg)

## Задание 3 — Курс валют через API ЦБ РФ



URL запроса: https://www.cbr.ru/scripts/XML_dynamic.asp?date_req1=15/05/2026&date_req2=30/05/2026&VAL_NM_RQ=R01235

![postman](.img/postman.jpg)
