# Сергей Ласточкин / Сергей Гончаров

Программист 1С, Санкт-Петербург. Работаю один и удалённо, так что пишете вы сразу тому, кто будет делать. Опишите задачу в двух-трёх предложениях в Telegram [t.me/metaanswer](https://t.me/metaanswer), отвечу, берусь или нет и как бы подошёл. Сайт - [lastochkin1c.ru](https://lastochkin1c.ru).

## Чем занимаюсь

Учёт управляющих компаний и ТСЖ, которые работают через ЕИРЦ или другой расчётный центр. Обычно в 1С у них не видно оплат жителей и перечислений агента, поэтому акты сверки и КУДиР не сходятся. Я сверяю отчёты агента с 1С и банком, нахожу, где и на сколько расходится, и восстанавливаю учёт за прошлые месяцы.

Генератор протоколов ОСС. Реестр собственников из экселя, повестка из готовых вопросов, а сообщение, бюллетени, реестр и протокол по приказу 44/пр собираются сами, с кворумом и итогами.

Маркировка «Честный знак» под ключ для селлеров: мойсклад, TopSeller, вб FBS, коды из сборки в отгрузку, вывод из оборота, дубли карточек.

Интеграции и автоматизация вокруг 1С: банк, н8н, маркетплейсы, загрузка выписок и данных поставщиков с проверками вместо ручного ввода. Если надо разобраться в чужой конфигурации, у меня есть свой [офлайн-поиск по BSL-коду](https://github.com/sergey-lastochkin/semantic-1c-code-search).

Работаю на тестовой копии базы, доступы и реквизиты в код и репозитории не попадают.

## Проекты

| Проект | Что это |
| --- | --- |
| [Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search) | Ищу по выгрузке конфигурации нужную процедуру и строки по вопросу, без интернета. Есть wheel для Windows, CI на Windows и Ubuntu, бенчмарк на 577 открытых BSL-файлах. |
| [Платёжный контур 1С](https://github.com/sergey-lastochkin/payment-integration-control-plane) | Повторы, статусы банка, сверка выписки и восстановление после сбоев, 18 сценариев сбоев и прогон через н8н. |
| [wb-moysklad-stock-sync](https://github.com/sergey-lastochkin/wb-moysklad-stock-sync) | Сверяю остатки вб с мойскладом и аккуратно снижаю лишнее на вб, только вниз и со снимком для отката. |
| [docgen](https://github.com/sergey-lastochkin/docgen) | Смета, договор, ТЗ и акт по заказу из одной строки. |
| [Process mining для 1С](https://github.com/sergey-lastochkin/process-mining-1c) | Где застревают согласования и возвраты, по журналу бизнес-событий, а не по ощущениям. |
| [Portfolio Risk API](https://github.com/sergey-lastochkin/portfolio-risk-api) | Сервис на FastAPI: VaR/CVaR, просадки и стресс-сценарии, есть [живое демо](https://portfolio-risk-api-eb40.onrender.com/?lang=ru). |
| [Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) | Конвейер и дашборд на открытых данных MOEX ISS. |

Стек: 1С (БП 3.0, ЖКХ 3.0, ЗУП, BSL, HTTP-сервисы), Python, FastAPI, н8н, JavaScript, SQLite/PostgreSQL, Docker, GitHub Actions.

<details>
<summary>English</summary>

Sergey Lastochkin - 1C:Enterprise developer and Python automation. Housing management accounting with payment agents, owners' meeting protocol generator, product marking (Chestny Znak) for marketplace sellers, bank and marketplace integrations, offline search across 1C configurations.
Contact: Telegram [t.me/metaanswer](https://t.me/metaanswer).

</details>
