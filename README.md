# Сергей Ласточкин 

Интеграции и автоматизация вокруг 1С и Python. Санкт-Петербург, работаю удалённо.

**Связаться: Telegram [@metaanswer](https://t.me/metaanswer)** — опишите задачу в
двух-трёх предложениях, отвечу, берусь ли и как бы подошёл.

## Чем могу помочь

- **Интеграция 1С с банком и внешними сервисами.** Заявка → платёжное поручение →
  отправка через n8n или свой сервис → статус обратно в 1С, без двойных платежей
  и потерянных статусов. Пример подхода — [платёжный контур](https://github.com/sergey-lastochkin/payment-integration-control-plane).
- **Автоматизация рутины в 1С.** Обработки, регламентные задания, HTTP-сервисы,
  загрузка данных поставщиков и выписок с проверками вместо ручного ввода.
- **Разбор чужой конфигурации.** Найти, где в коде живёт нужная логика, что
  затронет доработка, и оценить её до начала работ. Для этого у меня есть свой
  [офлайн-поиск по BSL-коду](https://github.com/sergey-lastochkin/semantic-1c-code-search).
- **Анализ процессов по данным 1С.** Где застревают согласования и возвраты — по
  журналу бизнес-событий, а не по ощущениям.

Работаю на тестовой копии базы, доступы и реквизиты в код и репозитории не
попадают.

## Проекты

| Проект | Что это |
| --- | --- |
| [Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search) | Локальный поиск по выгрузке конфигурации: процедура и строки по вопросу. Релиз с wheel для Windows, CI на Windows и Ubuntu, бенчмарк на 577 открытых BSL-файлах. |
| [Платёжный контур 1С](https://github.com/sergey-lastochkin/payment-integration-control-plane) | Повторы, статусы банка, сверка выписки и восстановление после сбоев; 18 сценариев сбоев и прогон через n8n. |
| [Process mining для 1С](https://github.com/sergey-lastochkin/process-mining-1c) | Варианты процесса, ожидания и возвраты; формат выгрузки бизнес-событий из 1С. |
| [Portfolio Risk API](https://github.com/sergey-lastochkin/portfolio-risk-api) | FastAPI-сервис VaR/CVaR, просадки и стресс-сценариев с [живым демо](https://portfolio-risk-api-eb40.onrender.com/?lang=ru). |
| [Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) | Конвейер и дашборд на публичных данных MOEX ISS. |

Стек: 1С (BSL, HTTP-сервисы), Python, FastAPI, n8n, SQLite/PostgreSQL, Docker,
GitHub Actions. 

<details>
<summary>English</summary>

Sergey Lastochkin — 1C:Enterprise and Python integrations and automation:
bank and external-service integrations for 1C, reliable payment exchange,
routine automation and code search across 1C configurations.
Main project: [Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search).
Contact: Telegram [@metaanswer](https://t.me/metaanswer).

</details>
