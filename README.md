# Сергей Гончаров

Интеграции и автоматизация вокруг 1С: Python-сервисы, API, очереди, внешние данные и инструменты для работы с BSL-кодом.

## Платёжный контур 1С

[payment-integration-control-plane](https://github.com/sergey-lastochkin/payment-integration-control-plane)

Разбираю путь платежа от заявки в 1С:УПП до банковского канала и обратного статуса. В коде уже есть модель операции, защита от повторной отправки, хранение попыток и правила переходов статуса. Следующий шаг – обезличенный прогон в тестовой базе УПП и проверка маршрута через n8n.

## Поиск и анализ связей в BSL-коде

[semantic-1c-code-search](https://github.com/sergey-lastochkin/semantic-1c-code-search) · [bsl-dependency-analyzer](https://github.com/sergey-lastochkin/bsl-dependency-analyzer)

Готовлю общий исследовательский проект по поиску процедур, зависимостей и оценке влияния изменений в выгрузках 1С. Публичные результаты будут основаны на открытом BSL-корпусе с зафиксированной лицензией, commit SHA и повторяемым benchmark-прогоном.

## Данные поставщиков

[supplier-data-pipeline](https://github.com/sergey-lastochkin/supplier-data-pipeline)

Пайплайн собирает карточки товаров, сохраняет снимки, нормализует поля и выносит неоднозначные совпадения на проверку. До размещения результатов на профиле он будет проверен на разрешённых публичных источниках, а не только на тестовых фикстурах.

## Анализ процессов 1С

[process-mining-1c](https://github.com/sergey-lastochkin/process-mining-1c)

Инструменты для вариантов процесса, длительностей, возвратов и отклонений от эталонной схемы. Следующий воспроизводимый запуск планируется на открытом event log; синтетические журналы останутся только в тестах формата.

## Другие работы

- [payroll-integration-control-plane](https://github.com/sergey-lastochkin/payroll-integration-control-plane) – контроль статусов и сверок вокруг 1С:ЗУП.
- [procurement-planning](https://github.com/sergey-lastochkin/procurement-planning) – расчёт потребности с учётом остатков, спроса и поставок.
- [master-data-resolution](https://github.com/sergey-lastochkin/master-data-resolution) – сопоставление контрагентов и номенклатуры с обработкой конфликтов.

## Дополнительный проект

[Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) – исследовательские пайплайны и отчёты на публичных данных MOEX. Это отдельная работа по данным, не основной фокус профиля.

## Контакт

Telegram: [@metaanswer](https://t.me/metaanswer)
