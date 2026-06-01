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



### GET через netcat

```bash
echo -e "GET / HTTP/1.1\r\nHost: example.com\r\n\r\n" | nc example.com 80
```

## Задание 2 — cURL

### GET запрос

```bash
curl -X GET "https://api.publicapis.org/entries?category=animals"
```

### POST запрос

```bash
curl -X POST "http://..." \
  -H "Content-Type: application/json" \
  -d '{"key": "value"}'
```

## Задание 3 — Курс валют через API ЦБ РФ



URL запроса: 