# Сергей Гончаров

Интеграции и автоматизация вокруг 1С: Python-сервисы, API, очереди, внешние данные и инструменты для работы с BSL-кодом.

## Поиск и анализ связей в BSL-коде

![Качество поиска в открытом BSL-корпусе](https://raw.githubusercontent.com/sergey-lastochkin/semantic-1c-code-search/main/studies/oss-bsl-corpus-2026-08-10/graphs/quality.svg)

[1C Code Intelligence](https://github.com/sergey-lastochkin/semantic-1c-code-search) ищет процедуры, связи и ссылки на метаданные в выгрузках 1С. Первый повторяемый прогон собран из 577 BSL-файлов трёх открытых проектов под Apache-2.0: 156869 строк и 7342 выделенных процедуры и функции.

**Проверено:** BM25 на 90 детерминированных проверках дал Recall@5 `0.855524`, MRR@10 `0.740384` и p95 `3.926` мс. Локальный hash-vector baseline показал худший результат; это зафиксировано в [results.json](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/studies/oss-bsl-corpus-2026-08-10/results.json).

[Исходники](https://github.com/sergey-lastochkin/semantic-1c-code-search) · [Корпус](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/docs/corpus.md) · [Ограничения парсера](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/docs/parser-limits.md)

## В работе

### Платёжный контур 1С

[payment-integration-control-plane](https://github.com/sergey-lastochkin/payment-integration-control-plane)

Разбираю путь от заявки в 1С:УПП до банковского канала и обратного статуса. В коде уже есть модель операции, защита от повторной отправки, хранение попыток и правила переходов статуса. Обезличенный запуск в тестовой УПП, маршрут n8n и банковский тестовый канал ещё не подтверждены, поэтому цифр и скриншотов здесь нет.

### Данные поставщиков

[supplier-data-pipeline](https://github.com/sergey-lastochkin/supplier-data-pipeline)

Пайплайн сохраняет снимки товаров, нормализует поля и выносит неоднозначные совпадения на проверку. Следующий результат будет основан на разрешённых публичных источниках, а не только на тестовых фикстурах.

### Анализ процессов 1С

[process-mining-1c](https://github.com/sergey-lastochkin/process-mining-1c)

Инструменты для вариантов процесса, длительностей, возвратов и отклонений от эталонной схемы. Воспроизводимый запуск на открытом event log ещё не опубликован.

## Дополнительные репозитории

- [payroll-integration-control-plane](https://github.com/sergey-lastochkin/payroll-integration-control-plane) – контроль статусов и сверок вокруг 1С:ЗУП.
- [procurement-planning](https://github.com/sergey-lastochkin/procurement-planning) – расчёт потребности с учётом остатков, спроса и поставок.
- [master-data-resolution](https://github.com/sergey-lastochkin/master-data-resolution) – сопоставление контрагентов и номенклатуры с обработкой конфликтов.
- [Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) – отдельная работа по публичным данным MOEX.

## Контакт

Telegram: [@metaanswer](https://t.me/metaanswer)
