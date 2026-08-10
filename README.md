# Сергей Гончаров

Интеграции и автоматизация вокруг 1С: Python-сервисы, API, очереди, внешние
данные и инструменты для работы с BSL-кодом.

## Платёжный контур 1С

![Результат локального failure lab](https://raw.githubusercontent.com/sergey-lastochkin/payment-integration-control-plane/main/failure_lab/runs/local-2026-08-10-01/report/failure-summary.svg)

[Payment Integration Control Plane](https://github.com/sergey-lastochkin/payment-integration-control-plane)
разбирает путь от заявки в 1С:УПП до банковского статуса: business operation,
повторная отправка, callback, сверка и ручное завершение спорной операции.
Коммерческий контекст обезличен: производственная компания, УПП, несколько
банковских каналов и n8n.

**Проверено локально:** 13 сценариев сбоев завершились без двойной операции,
включая callback до ответа отправителя, повтор статуса, потерю ответа и
неоднозначную выписку. Это не подтверждение запуска в тестовой УПП, n8n или
банковском канале: такие доказательства ещё не опубликованы.

[Исходники](https://github.com/sergey-lastochkin/payment-integration-control-plane) · [Сценарии](https://github.com/sergey-lastochkin/payment-integration-control-plane/tree/main/failure_lab/runs/local-2026-08-10-01) · [Ограничения](https://github.com/sergey-lastochkin/payment-integration-control-plane/blob/main/docs/operations.md)

## Поиск и анализ связей в BSL-коде

![Качество поиска в открытом BSL-корпусе](https://raw.githubusercontent.com/sergey-lastochkin/semantic-1c-code-search/main/studies/oss-bsl-corpus-2026-08-10/graphs/quality.svg)

[1C Code Intelligence](https://github.com/sergey-lastochkin/semantic-1c-code-search)
ищет процедуры, связи и ссылки на метаданные. Корпус собран из 577 BSL-файлов
трёх открытых Apache-2.0 проектов: 156 869 строк и 7 342 выделенных процедуры
и функции.

**Проверено:** BM25 на 90 детерминированных запросах дал Recall@5 `0.855524`,
MRR@10 `0.740384` и p95 `3.926` мс. Локальный hash-vector baseline оказался
хуже, что сохранено в результатах.

[Исходники](https://github.com/sergey-lastochkin/semantic-1c-code-search) · [Результаты](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/studies/oss-bsl-corpus-2026-08-10/results.json) · [Ограничения парсера](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/docs/parser-limits.md)

## Данные поставщиков

![Результат обхода каталогов](https://raw.githubusercontent.com/sergey-lastochkin/supplier-data-pipeline/main/studies/openfacts-catalog-run-2026-08-10/graphs/source-metrics.svg)

[Supplier Data Pipeline](https://github.com/sergey-lastochkin/supplier-data-pipeline)
получает каталог, проверяет схему, сохраняет snapshot и дельты, а слабые
совпадения отправляет на ручную проверку. Первый read-only run использует Open
Food Facts, Open Beauty Facts и Open Pet Food Facts.

**Проверено:** из 36 полученных записей приняты 26; 10 без `product_name`
отклонены до commit. Запуск занял 15.162 секунды и завершился без ошибок
источников. Точный cross-source match в этой небольшой выборке не встретился.

[Исходники](https://github.com/sergey-lastochkin/supplier-data-pipeline) · [Результаты](https://github.com/sergey-lastochkin/supplier-data-pipeline/blob/main/studies/openfacts-catalog-run-2026-08-10/results.json) · [Источники](https://github.com/sergey-lastochkin/supplier-data-pipeline/blob/main/docs/source-policy.md)

## Анализ процессов для будущей выгрузки 1С

![Варианты и ожидания BPI Challenge 2012](https://raw.githubusercontent.com/sergey-lastochkin/process-mining-1c/main/studies/bpi-challenge-2012-2026-08-10/graphs/variants-bottlenecks.svg)

[Process Mining for 1C](https://github.com/sergey-lastochkin/process-mining-1c)
задаёт контракт бизнес-событий для 1С и проверяет методы на полном открытом
XES-журнале BPI Challenge 2012. Публичный журнал не выдаётся за журнал 1С,
а самый частый вариант используется только как статистический baseline.

**Проверено:** 262 200 событий, 13 087 cases, 24 действия, 4 366 вариантов и
125 переходов обработаны за 10.235 секунды. p95 длительности case составил
31.343 суток; причина задержек по одному журналу не утверждается.

[Исходники](https://github.com/sergey-lastochkin/process-mining-1c) · [Результаты](https://github.com/sergey-lastochkin/process-mining-1c/blob/main/studies/bpi-challenge-2012-2026-08-10/results.json) · [Методика](https://github.com/sergey-lastochkin/process-mining-1c/blob/main/docs/study-design.md)

## Дополнительно

- [Procurement Planning](https://github.com/sergey-lastochkin/procurement-planning) – правила потребности и ограничений поставщика; есть отдельный bounded snapshot публичного API ProZorro, который не подменяет supplier catalog.
- [Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) – отдельный проект на публичных данных MOEX.

## Контакт

Telegram: [@metaanswer](https://t.me/metaanswer)
