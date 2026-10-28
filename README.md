# Сергей Ласточкин / Сергей Гончаров

программист 1С, Санкт-Петербург. работаю один и удалённо, так что пишете вы сразу тому, кто будет делать. опишите задачу в двух-трёх предложениях в Telegram [t.me/metaanswer](https://t.me/metaanswer), отвечу, берусь или нет и как бы подошёл. сайт - [lastochkin1c.ru](https://lastochkin1c.ru).

## стек

#### 1С

<img src="badges/1-ebe4.svg" alt="1С:Предприятие" height="28"> <img src="badges/3-0-0009.svg" alt="БП 3.0" height="28"> <img src="badges/3-0-7d4d.svg" alt="ЖКХ 3.0" height="28"> <img src="badges/22e0.svg" alt="ЗУП" height="28"> <img src="badges/bsl-7f6f.svg" alt="BSL" height="28"> <img src="badges/http-8888.svg" alt="HTTP-сервисы" height="28">

#### языки

<img src="badges/python-a7f5.svg" alt="Python" height="28"> <img src="badges/typescript-558b.svg" alt="TypeScript" height="28"> <img src="badges/javascript-6861.svg" alt="JavaScript" height="28"> <img src="badges/swift-ae83.svg" alt="Swift" height="28"> <img src="badges/sql-9778.svg" alt="SQL" height="28"> <img src="badges/bash-7024.svg" alt="Bash" height="28"> <img src="badges/powershell-3d26.svg" alt="PowerShell" height="28"> <img src="badges/html-css-688d.svg" alt="HTML/CSS" height="28">

#### фреймворки и данные

<img src="badges/fastapi-f275.svg" alt="FastAPI" height="28"> <img src="badges/react-native-bd9b.svg" alt="React Native" height="28"> <img src="badges/expo-c29f.svg" alt="Expo" height="28"> <img src="badges/swiftui-5d80.svg" alt="SwiftUI" height="28"> <img src="badges/postgresql-399b.svg" alt="PostgreSQL" height="28"> <img src="badges/sqlite-4977.svg" alt="SQLite" height="28"> <img src="badges/drizzle-5bfc.svg" alt="Drizzle" height="28">

#### интеграции и автоматизация

<img src="badges/n8n-5877.svg" alt="n8n" height="28"> <img src="badges/wildberries-ba49.svg" alt="Wildberries" height="28"> <img src="badges/2b56.svg" alt="МойСклад" height="28"> <img src="badges/514d.svg" alt="Честный знак" height="28"> <img src="badges/playwright-26d8.svg" alt="Playwright" height="28">

#### инфраструктура

<img src="badges/docker-c5fd.svg" alt="Docker" height="28"> <img src="badges/github-actions-f843.svg" alt="GitHub Actions" height="28"> <img src="badges/linux-edc9.svg" alt="Linux" height="28"> <img src="badges/macos-8b06.svg" alt="macOS" height="28"> <img src="badges/xray-b99f.svg" alt="Xray" height="28"> <img src="badges/claude-code-38c6.svg" alt="Claude Code" height="28"> <img src="badges/git-0bcc.svg" alt="Git" height="28">

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

<details>
<summary>English</summary>

Sergey Lastochkin - 1C:Enterprise developer and Python automation. Housing management accounting with payment agents, owners' meeting protocol generator, product marking (Chestny Znak) for marketplace sellers, bank and marketplace integrations, offline search across 1C configurations.
Contact: Telegram [t.me/metaanswer](https://t.me/metaanswer).

</details>
