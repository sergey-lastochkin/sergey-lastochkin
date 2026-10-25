# Сергей Ласточкин / Сергей Гончаров

программист 1С, Санкт-Петербург. работаю один и удалённо, так что пишете вы сразу тому, кто будет делать. опишите задачу в двух-трёх предложениях в Telegram [t.me/metaanswer](https://t.me/metaanswer), отвечу, берусь или нет и как бы подошёл. 

## чем занимаюсь

учёт управляющих компаний и ТСЖ, которые работают через ЕИРЦ или другой расчётный центр. обычно в 1С у них не видно оплат жителей и перечислений агента, поэтому акты сверки и КУДиР не сходятся. я сверяю отчёты агента с 1С и банком, нахожу, где и на сколько расходится, и восстанавливаю учёт за прошлые месяцы.

генератор протоколов ОСС. реестр собственников из экселя, повестка из готовых вопросов, а сообщение, бюллетени, реестр и протокол по приказу 44/пр собираются сами, с кворумом и итогами.

маркировка «Честный знак» под ключ для селлеров: мойсклад, TopSeller, вб FBS, коды из сборки в отгрузку, вывод из оборота, дубли карточек.

интеграции и автоматизация вокруг 1С: банк, н8н, маркетплейсы, загрузка выписок и данных поставщиков с проверками вместо ручного ввода. если надо разобраться в чужой конфигурации, у меня есть свой [офлайн-поиск по BSL-коду](https://github.com/sergey-lastochkin/semantic-1c-code-search).

работаю на тестовой копии базы, доступы и реквизиты в код и репозитории не попадают.

## проекты

| проект | что это |
| --- | --- |
| [Semantic 1C Code Search](https://github.com/sergey-lastochkin/semantic-1c-code-search) | ищу по выгрузке конфигурации нужную процедуру и строки по вопросу, без интернета. есть wheel для Windows, CI на Windows и Ubuntu, бенчмарк на 577 открытых BSL-файлах. |
| [Платёжный контур 1С](https://github.com/sergey-lastochkin/payment-integration-control-plane) | повторы, статусы банка, сверка выписки и восстановление после сбоев, 18 сценариев сбоев и прогон через н8н. |
| [wb-moysklad-stock-sync](https://github.com/sergey-lastochkin/wb-moysklad-stock-sync) | сверяю остатки вб с мойскладом и аккуратно снижаю лишнее на вб, только вниз и со снимком для отката. |
| [docgen](https://github.com/sergey-lastochkin/docgen) | смета, договор, ТЗ и акт по заказу из одной строки. |
| [Process mining для 1С](https://github.com/sergey-lastochkin/process-mining-1c) | где застревают согласования и возвраты, по журналу бизнес-событий, а не по ощущениям. |
| [Portfolio Risk API](https://github.com/sergey-lastochkin/portfolio-risk-api) | сервис на FastAPI: VaR/CVaR, просадки и стресс-сценарии, есть [живое демо](https://portfolio-risk-api-eb40.onrender.com/?lang=ru). |
| [Russian Markets Lab](https://github.com/sergey-lastochkin/russian-markets-lab) | конвейер и дашборд на открытых данных MOEX ISS. |

стек: 1С (БП 3.0, ЖКХ 3.0, ЗУП, BSL, HTTP-сервисы), Python, FastAPI, н8н, JavaScript, SQLite/PostgreSQL, Docker, GitHub Actions.

<details>
<summary>English</summary>

Sergey Lastochkin - 1C:Enterprise developer and Python automation. Housing management accounting with payment agents, owners' meeting protocol generator, product marking (Chestny Znak) for marketplace sellers, bank and marketplace integrations, offline search across 1C configurations.
Contact: Telegram [t.me/metaanswer](https://t.me/metaanswer).

</details>
