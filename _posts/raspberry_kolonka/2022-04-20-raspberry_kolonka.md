---
layout: post
title:  "Raspberry Pi + Колонка"
date:   2022-04-20 19:24:00 +0300
tags: [Raspberry Pi, linux]
---

- Решение для воспроизведения музыки на мероприятих / переменах 
### Принцип работы:
- Загружаете mp3 файлы, сохраняете в playlist.m3u
- На распбери с автозагрузки запускается VLC и открывает этот плейлист
- В заданное в кроне время запускаются скрипты то на включение, то на выключение звука

### Установка
Скачать репозиторий

```bash
$ git clone https://qweqwe.github.com
```

### Конфигурация

Настроить крон

```bash
$ crontab -e
```

Раскидать файлы по каталогам

Загрузить музыку

Создать плейлист

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
