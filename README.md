# Сергей Гончаров · Sergey Goncharov

Разрабатываю open-source инструменты для поиска и анализа BSL-кода, оценки
влияния изменений и надёжных интеграций вокруг 1С и Python.

Building practical open-source tools for 1C/BSL code search, change-impact
analysis, and integration reliability.

## Главный проект

### [Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search)

Локальный поиск по выгруженной конфигурации: BM25 для точных терминов и
опциональные multilingual embeddings для вопросов на естественном языке.
Показывает модуль и строки, не требует запущенной платформы 1С и не отправляет
BSL-код во внешний API.

[![CI](https://github.com/sergey-lastochkin/semantic-1c-code-search/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sergey-lastochkin/semantic-1c-code-search/actions/workflows/ci.yml)
[![License: Apache-2.0](https://img.shields.io/badge/license-Apache--2.0-green.svg)](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/LICENSE)

```bash
code-search search /path/to/config-export "СформироватьНазначениеПлатежа"
```

Benchmark построен на 577 открытых BSL-файлах и 156 869 строках. Результаты,
исходные revision и хэши опубликованы вместе с кодом.

## Ещё два инструмента для 1С-разработки

| Проект | Что решает |
| --- | --- |
| [BSL Dependency Analyzer](https://github.com/sergey-lastochkin/bsl-dependency-analyzer) | Строит статический граф зависимостей, blast radius и кандидатов для регрессионной проверки. |
| [1C Integration Observability](https://github.com/sergey-lastochkin/integration-observability) | Связывает одну операцию между 1С, n8n и Python: traces, retries, DLQ, replay и группировка инцидентов. |

## Другие работы

- [Process Mining и события 1С](https://github.com/sergey-lastochkin/process-mining-1c) — варианты процессов, ожидания и возвраты по журналам событий.
- [Payment Integration Control Plane](https://github.com/sergey-lastochkin/payment-integration-control-plane) — повторные запросы, банковские статусы, сверка и восстановление после сбоев.
- [Portfolio Risk API](https://github.com/sergey-lastochkin/portfolio-risk-api) — FastAPI-сервис для VaR/CVaR, drawdown, концентрации и stress scenarios.

## Темы

`1C` · `BSL` · `Python` · `code search` · `static analysis` · `integration reliability`

Telegram: [@metaanswer](https://t.me/metaanswer)
