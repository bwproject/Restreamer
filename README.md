<!--
  ВНИМАНИЕ: этот файл изменён по сравнению с оригиналом.
  Это русский перевод README проекта datarhei/restreamer.
  Оригинал: https://github.com/datarhei/restreamer — ветка 2.x, коммит fd12aee
  Оригинальный английский текст без изменений: README.en.md
  Лицензия оригинала: Apache License 2.0 — см. файл LICENSE.
  Перечень изменений: файл NOTICE.
-->

<h1 align="center">Restreamer</h1>
<h3 align="center">По-настоящему удобная и бесплатная альтернатива для работы с прямыми трансляциями.</h3>
<p align="center">
<a href="https://github.com/bwproject/Restreamer/blob/main/LICENSE" target="_blank"><img src="https://img.shields.io/github/license/bwproject/Restreamer" alt="Лицензия" /></a>
<a href="https://github.com/bwproject/Restreamer/releases" target="_blank"><img src="https://img.shields.io/github/v/release/bwproject/Restreamer?include_prereleases" alt="Релиз" /></a>
<a href="https://hub.docker.com/r/datarhei/restreamer" target="_blank"><img src="https://img.shields.io/docker/pulls/datarhei/restreamer" alt="Загрузки Docker-образа" /></a>
<a href="https://docs.datarhei.com/restreamer/getting-started/quick-start" target="_blank"><img src="https://img.shields.io/badge/%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D1%8F-%D1%81%20%D1%87%D0%B5%D0%B3%D0%BE%20%D0%BD%D0%B0%D1%87%D0%B0%D1%82%D1%8C-green" alt="Документация" /></a>
</p>
<p align="center"><a href="https://demo.datarhei.com/ui" target="_blank">Посмотреть живое демо</a><br />
<a href="https://demo.datarhei.com/ui" target="_blank"><img src="https://img.shields.io/badge/%D0%BB%D0%BE%D0%B3%D0%B8%D0%BD-admin-blue" alt="логин для демо" /></a>
<a href="https://demo.datarhei.com/ui" target="_blank"><img src="https://img.shields.io/badge/%D0%BF%D0%B0%D1%80%D0%BE%D0%BB%D1%8C-demo-blue" alt="пароль для демо" /></a>

---

## 📖 О переводе, источнике и лицензии

**Это неофициальный русский перевод документации проекта Restreamer.**

| | |
|---|---|
| **Оригинальный проект** | [datarhei/restreamer](https://github.com/datarhei/restreamer) |
| **Авторы оригинала** | datarhei GmbH и участники проекта (см. историю коммитов и `LICENSE`) |
| **Ветка / коммит перевода** | `2.x`, `fd12aee` («Bundle with FFmpeg 8») |
| **Лицензия оригинала** | [Apache License 2.0](./LICENSE) |
| **Что переведено** | только этот файл, `README.md`. Оригинальный английский текст сохранён без изменений в [`README.en.md`](./README.en.md) |
| **Что изменено** | см. [`NOTICE`](./NOTICE) — там перечислены все правки относительно оригинала |

Оригинальный текст распространяется под лицензией **Apache License, Version 2.0**.
В соответствии с её условиями в этом репозитории сохранены файл `LICENSE`, все
уведомления об авторских правах и перечень внесённых изменений (`NOTICE`).
Перевод является производной работой и распространяется под той же лицензией
Apache-2.0.

**Товарные знаки.** Названия «datarhei» и «Restreamer», логотипы и оформление
принадлежат их правообладателям. Лицензия Apache-2.0 не даёт прав на использование
товарных знаков. Этот репозиторий **не является официальным** и не связан с
datarhei GmbH, не одобрен и не поддерживается ею. Официальный источник —
[datarhei/restreamer](https://github.com/datarhei/restreamer), официальная
документация — [docs.datarhei.com/restreamer](https://docs.datarhei.com/restreamer).

---

<p align="center">
  <a href="https://datarhei.com">
    <img src="./readme-promo.gif" alt="Промо-ролик Restreamer" />
  </a>
</p>

<p align="center">Решение для самостоятельного размещения (self-hosting), которое позволяет вести прямые трансляции на свой сайт и публиковать их на множестве платформ — YouTube-Live, Twitter, Twitch, Vimeo и других сервисах. Наш Docker-образ прост в установке и работает в Linux-окружениях (MacOS/Windows — через Docker Desktop). Кроме того, Restreamer можно совмещать с одноплатными компьютерами вроде Raspberry Pi или с системами, где видео кодируется на GPU.</p>
<br />
<hr />

## Возможности

- Упрощённый пользовательский интерфейс
- Простой мастер настройки
- Несколько источников аудио/видео, выходов, протоколов и кодеков
- Рестриминг на платформы вроде YouTube-Live, в программы вроде Wowza Media Server и другие — по протоколам RTMP, SRT, ...
- Возможность подмешать отдельную аудиодорожку к видео
- Встроенный плеер VideoJS для вашего сайта
- Настраиваемая страница публикации для трансляции без встраивания плеера
- Лицензирование контента через Creative Commons
- Потоковый сервер HTTP/S (HLS), RTMP/S и SRT
- Автоматическое получение HTTPS-сертификатов Let's Encrypt
- Мониторинг и ограничение числа зрителей и полосы пропускания
- Поддержка Raspberry Pi (MMAL/OMX), Nvidia CUDA, Intel VAAPI
- Поддержка аппаратных и виртуальных устройств
- Обработка видео через FFmpeg (максимально нативно)
- REST-API (JSON) со 100% документацией в Swagger
- Мониторинг ресурсов (опционально — через метрики Prometheus)
- Логирование сервера и процессов
- Соответствие GDPR: без сторонних провайдеров, данные зрителей не сохраняются

## Быстрая установка

### AMD64/ARMv7/ARM64:
```sh
docker run -d --restart=always --name restreamer \
   -v /opt/restreamer/config:/core/config -v /opt/restreamer/data:/core/data \
   -p 8080:8080 -p 8181:8181 \
   -p 1935:1935 -p 1936:1936 \
   -p 6000:6000/udp \
   datarhei/restreamer:latest
```

*Флаг `--privileged` нужен только для локальных устройств вроде USB-камер.*
*Если ни один сетевой источник недоступен, попробуйте `--security-opt seccomp=unconfined`.*

### ARMv7/ARM64 Raspberry Pi:
```sh
docker run -d --restart=always --name restreamer \
   -v /opt/restreamer/config:/core/config -v /opt/restreamer/data:/core/data \
   --privileged \
   -p 8080:8080 -p 8181:8181 \
   -p 1935:1935 -p 1936:1936 \
   -p 6000:6000/udp \
   datarhei/restreamer:rpi-latest
```

*Флаг `--privileged` нужен только для локальных устройств вроде USB-камер.*
*Если ни один сетевой источник недоступен, попробуйте `--security-opt seccomp=unconfined`.*

### AMD64 Nvidia CUDA:
```sh
docker run -d --restart=always --name restreamer \
   -v /opt/restreamer/config:/core/config -v /opt/restreamer/data:/core/data \
   --runtime=nvidia --privileged \
   -p 8080:8080 -p 8181:8181 \
   -p 1935:1935 -p 1936:1936 \
   -p 6000:6000/udp \
   datarhei/restreamer:cuda-latest
```

*Флаг `--privileged` нужен только для локальных устройств вроде USB-камер.*
*Если ни один сетевой источник недоступен, попробуйте `--security-opt seccomp=unconfined`.*

### AMD64 Intel VAAPI:
```sh
docker run -d --restart=always --name restreamer \
   -v /opt/restreamer/config:/core/config -v /opt/restreamer/data:/core/data \
   -v /dev/dri:/dev/dri --privileged \
   -p 8080:8080 -p 8181:8181 \
   -p 1935:1935 -p 1936:1936 \
   -p 6000:6000/udp \
   datarhei/restreamer:vaapi-latest
```

*Флаг `--privileged` нужен только для локальных устройств вроде USB-камер.*
*Если ни один сетевой источник недоступен, попробуйте `--security-opt seccomp=unconfined`.*

*Для доступа извне (http/s, rtmp/s, srt) может потребоваться проброс портов на интернет-роутере на внутренний IP-адрес Restreamer.*

## Документация

Документация доступна на [docs.datarhei.com/restreamer](https://docs.datarhei.com/restreamer) (на английском языке). Там подробно описано многое: от подключения камеры и встраивания плеера на свой сайт до трансляции на сервисы вроде YouTube-Live и не только.

- [С чего начать](https://docs.datarhei.com/restreamer/getting-started/quick-start)
- [Установка](https://docs.datarhei.com/restreamer/installing/minimum-requirements)
- [Руководство](https://docs.datarhei.com/restreamer/knowledge-base/manual)
- [Инструкции](https://docs.datarhei.com/restreamer/knowledge-base/user-guides)

## Разработка

### Сборка собственного образа (bundle):

#### [Restreamer FFmpeg](https://github.com/datarhei/ffmpeg):
```
$ git clone github.com/datarhei/ffmpeg
$ cd ffmpeg
$ docker build -f Dockerfile.alpine -t myffmpeg .
```

#### [Бэкенд Restreamer](https://github.com/datarhei/core) (Golang):

```
$ git clone github.com/datarhei/core
$ cd core
$ docker build -t mycore .
```

#### [Интерфейс Restreamer](https://github.com/datarhei/restreamer-ui) (React):
```
$ git clone github.com/datarhei/restreamer-ui
$ cd restreamer-ui
$ docker build -t myrsui .
```

#### Сборка самого Restreamer:
```
$ git clone github.com/datarhei/restreamer
$ cd restreamer
$ docker build --build-arg FFMPEG_IMAGE=myffmpeg --build-arg CORE_IMAGE=mycore --build-arg RESTREAMER_UI_IMAGE=myrsui -t myrestreamer .
$ docker run -it --rm -p 8080:8080 myrestreamer
```

### Как добавить или исправить переводы в [интерфейсе Restreamer](https://github.com/datarhei/restreamer-ui):

Интерфейс Restreamer уже переведён на разные языки, включая немецкий, французский, итальянский, испанский и другие. Если вы нашли ошибку в переводе или у вас есть вариант получше для какой-то фразы, вы можете стать переводчиком на [poeditor.com](https://poeditor.com/join/project/ogATl3F48K).
Там же можно начать перевод на язык, которого в интерфейсе Restreamer ещё нет.

Участвовать в переводах: [https://poeditor.com/join/project/ogATl3F48K](https://poeditor.com/join/project/ogATl3F48K)

## Сборка в этом репозитории (GitHub Actions)

> ⚙️ Этот раздел добавлен в форк — в оригинальном README его нет.

Образы, собранные в этом репозитории, публикуются в **GitHub Container Registry**:

```
ghcr.io/bwproject/restreamer:latest    # bundle, amd64
ghcr.io/bwproject/restreamer:dev       # dev-сборка (UI: dev)
```

Команды из раздела «Быстрая установка» выше используют **официальные** образы
`datarhei/restreamer`. Чтобы запустить образ из этого репозитория, замените имя:

```sh
docker run -d --restart=always --name restreamer \
   -v /opt/restreamer/config:/core/config -v /opt/restreamer/data:/core/data \
   -p 8080:8080 -p 8181:8181 \
   -p 1935:1935 -p 1936:1936 \
   -p 6000:6000/udp \
   ghcr.io/bwproject/restreamer:latest
```

Workflows:

| Workflow | Когда запускается | Что делает |
|---|---|---|
| `CI: build image` | push в `main`/`2.x`, pull request | собирает образ и прогоняет smoke-тест (FFmpeg, раскладка `/core`) |
| `Build restreamer latest images` | вручную, push тега `v*` | собирает 4 варианта (default, rpi, vaapi, cuda) и публикует в GHCR |
| `Build restreamer dev images` | вручную, ежедневно в 05:37 UTC | собирает dev-варианты и публикует теги `*-dev` |

Каждый вариант собирается только под те архитектуры, которые есть у его базовых
образов: default — `linux/amd64`, `linux/arm64`, `linux/arm/v7`; rpi — arm64/armv7;
vaapi и cuda — amd64. Arch-и, отличные от amd64, собираются через QEMU. При ручном
запуске можно снять флажок `multiarch` — тогда каждый вариант соберётся под одну
архитектуру и сборка пройдёт быстрее.

Все сборки идут на стандартных GitHub-раннерах (`ubuntu-latest`), никакие
self-hosted раннеры и секреты не требуются: для GHCR используется встроенный
`GITHUB_TOKEN`. Если дополнительно нужен Docker Hub, задайте переменную
репозитория `DOCKERHUB_IMAGE` (например, `bwproject/restreamer`) и секреты
`DOCKERHUB_USERNAME` / `DOCKERHUB_TOKEN`.

## Поддержка сообщества

По общим вопросам использования Restreamer обращайтесь к официальной [документации](https://docs.datarhei.com/restreamer). Дополнительно можно задать вопрос на GitHub (сообщения об ошибках, предложения, обсуждение возможностей).

## Лицензия

Проект распространяется по лицензии **Apache License, Version 2.0**.
Полный текст — в файле [`LICENSE`](./LICENSE), сведения о происхождении и
перечень изменений — в файле [`NOTICE`](./NOTICE).

Оригинал: [datarhei/restreamer](https://github.com/datarhei/restreamer) —
Copyright 2022 FOSS GmbH и участники проекта. Все права сохранены за их
правообладателями. Перевод и правки в этом репозитории распространяются под той
же лицензией Apache-2.0.

## Коммерческие вопросы

**Мы предоставляем поддержку коммерческих задач: профессиональный саппорт, гибкую разработку и консалтинг.** Если у вас есть коммерческий запрос — будь то ошибка или доработка функциональности, — напишите напрямую на support@datarhei.com.
