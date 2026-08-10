# Сергей Гончаров

Разрабатываю интеграции вокруг 1С и Python. Работаю с HTTP API, внешними
сервисами, очередями, банковскими интеграциями и инструментами для анализа
BSL-кода.

## Платёжный контур 1С

![Итог локального прогона сценариев сбоев](https://raw.githubusercontent.com/sergey-lastochkin/payment-integration-control-plane/main/failure_lab/runs/local-2026-08-10-01/report/failure-summary.svg)

[Payment Integration Control Plane](https://github.com/sergey-lastochkin/payment-integration-control-plane) описывает путь заявки из 1С:УПП до банковского статуса. В локальном прогоне проверены 13 сценариев сбоев: повтор запроса, потеря ответа, двойной статус, повтор выписки и неоднозначная сверка.

Повтор не создаёт две операции. Неоднозначная сверка требует ручной проверки. Тестовая УПП, n8n и банковский канал ещё не подключались; для них подготовлен [чек-лист и журнал прогона](https://github.com/sergey-lastochkin/payment-integration-control-plane/tree/main/real_run).

[Код и результаты](https://github.com/sergey-lastochkin/payment-integration-control-plane) · [границы прогона](https://github.com/sergey-lastochkin/payment-integration-control-plane/blob/main/docs/operations.md)

## Поиск по BSL-коду

![Локальный поиск по BSL-корпусу](https://raw.githubusercontent.com/sergey-lastochkin/semantic-1c-code-search/main/assets/search-example.png)

[Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search) проверен на 577 BSL-файлах и 156869 строках трёх открытых Apache-2.0 проектов. В корпусе выделено 7342 процедуры и функции.

На 90 точных проверках лучший Recall@5 у BM25: `0.855524`. RRF с локальными эмбеддингами дал лучший MRR@10: `0.788470`. На 42 русских вопросах эмбеддинги выше BM25, но их разметка ещё требует ручной проверки и не выдаётся за окончательную метрику.

[Код](https://github.com/sergey-lastochkin/semantic-1c-code-search) · [результаты](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/studies/oss-bsl-corpus-2026-08-10/embedding-results.json) · [границы парсера](https://github.com/sergey-lastochkin/semantic-1c-code-search/blob/main/docs/parser-limits.md)

## Анализ процессов

![Частые варианты и длинные ожидания BPI Challenge 2012](https://raw.githubusercontent.com/sergey-lastochkin/process-mining-1c/main/studies/bpi-challenge-2012-2026-08-10/graphs/variants-bottlenecks.svg)

[Process Mining и события 1С](https://github.com/sergey-lastochkin/process-mining-1c) считает варианты, ожидания и возвраты в журналах событий. Алгоритмы проверены на полном открытом BPI Challenge 2012: 262200 событий, 13087 случаев, 4366 вариантов.

BPI не является журналом 1С. В проекте отдельно описан контракт событий для выгрузки из 1С, поскольку одного журнала регистрации недостаточно для бизнес-интерпретации.

[Код](https://github.com/sergey-lastochkin/process-mining-1c) · [результаты](https://github.com/sergey-lastochkin/process-mining-1c/blob/main/studies/bpi-challenge-2012-2026-08-10/results.json) · [контракт событий](https://github.com/sergey-lastochkin/process-mining-1c/blob/main/onec_export/event-contract.md)

## Russian Markets Lab

![Панель исторических данных MOEX](https://raw.githubusercontent.com/sergey-lastochkin/russian-markets-lab/main/assets/readme_dashboard_overview.png)

[Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) собирает диагностики ликвидности, фьючерсного базиса и исторического риска по публичному MOEX ISS. Сохранённый набор содержит 6 таблиц и 260 строк.

На скриншоте и в данных указана дата `2026-06-19`. Это исторический снимок, а не текущая рыночная картина; брокерского исполнения и торговых рекомендаций в проекте нет.

[Код](https://github.com/sergey-lastochkin/russian-markets-lab) · [источники](https://github.com/sergey-lastochkin/russian-markets-lab/blob/main/docs/data_sources.md) · [ограничения](https://github.com/sergey-lastochkin/russian-markets-lab/blob/main/docs/limitations.md)

## Другие проекты

- [Supplier Data Pipeline](https://github.com/sergey-lastochkin/supplier-data-pipeline): импорт из трёх открытых товарных каталогов, 36 записей получено, 26 прошли проверку схемы.
- [Procurement Planning](https://github.com/sergey-lastochkin/procurement-planning): правила потребности и ограничений поставщика, результаты определения поставщика через публичный API ProZorro.

## Контакт

Telegram: [@metaanswer](https://t.me/metaanswer)
