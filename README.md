# Yandex

## Навигация
* [Описание ](#Описание)
* [Подключение Яндекс.Метрики в личном кабинете CallKeeper](#Подключение-Яндекс.Метрики-в-личном-кабинете-CallKeeper)
* [Настройки счётчиков ](#Настройки-счётчиков)
* [Отчеты ](#Отчеты)

## Описание

Интеграция позволяет отправлять звонки динамического и статического коллтрекинга, а также обратные звонки CallKeeper и их параметры в стандартные отчеты по звонкам в Яндекс.Метрику.

Чтобы настроить передачу данных, необходимо авторизоваться в аккаунте Яндекс.Метрики https://metrika.yandex.ru/ под правами администратора или редактора.
 

## Подключение Яндекс.Метрики в личном кабинете CallKeeper

Для подключения интеграции необходимо:

1. Зайти в свой личный кабинет на https://ckct.ru/ :

![Рис.1](images/LK_CT_1.jpg)

2. Перейдите по ссылке https://ckct.ru/dev/lk/integrations в раздел Интеграции в личном кабинете Callkeeper и нажать подключить:

![Рис.2](images/yan_in_1.jpg)

3. Откроется окно авторизации Яндекс , где необходимо ввести данные аккаунта под которым вы хотите войти:

![Рис.5](images/login_1.jpg)

4. После этого откроется странница на который необходимо выбрать счетчики которые вы хотите добавить: 

![Рис.6](images/shetshik.png)

## Настройки счётчиков

Для настройки счётчиков необходимо нажать на его название и откроется окно настройки : 

![Рис.8](images/seting.png)

Где вы сможете выставить настройки под нужные вам параментры.

После выставления настроек их необходимо сохранить :

## Настройка целей 

Если необходимо настроить цель по отправки всех звонков в яндекс.метрику необходимо : 

1) создать цель на стороне яндекс.метрики 
2) Выбрать цель для отправки событий в настройках счетчика на стороне CallKeeper 

![Рис.8](images/1234.jpg)

В качестве достижения цели будет передаваться количество всех звонков (удачные+неудачные). 


## Отчеты
Передаваемые данные собираются в отдельную группу отчетов в Яндекс.Метрике: «Качество обработки звонков», «Источники звонков», «Звонки, детально».

![Рис.9](images/Zvonki-SHag1.png)

Отчет **ачество обработки звонков»** казывает длительность звонка и долю пропущенных звонков. Данные помогут проанализировать эффективность работы менеджеров или коллцентра.

![Рис.9](images/kachestvo-obrabotki-zvonkov-1.png)

![Рис.9](images/kachestvo-2.png)

Отчет **«Источники звонков»** показывает подробности о посетителях и их поведении на сайте. Отображает данные только по звонкам динамического коллтрекинга.

![Рис.9](images/Istochniki-1.png)

![Рис.9](images/Istochniki-2.png)

Отчет **«Звонки, детально»** является основным отчетом о звонках, отображает данные динамического и статического коллтрекинга. Содержит информацию о дате/времени звонка, длительности разговора, номере телефона клиента, статуса звонка: первичный/вторичный, источника трафика, который привел к звонку и другие параметры.

![Рис.9](images/zvonki_-detalno.png)

Статус звонка «привязанный/непривязанный» показывает наличие сессии у звонка. Если произошла ошибка привязки, и статус отобразился как «непривязанный», то это значит, что Яндекс.Метрика не нашла уникальный идентификатор ClientID. Это может произойти в случае звонка на статический номер или нехватки номеров, также, если пользователь совершил звонок, не заходя на сайт (записал номер телефона и перезвонил по нему, не посещая сайт). Ошибка привязки сессии может быть также в случае, если на сайте не установлен счетчик Яндекс.Метрики или установлен некорректно, либо блокируется сторонними сервисами.
После интеграции во вкладке Цели появится автоматически созданная Яндекс.Метрикой цель «Звонок»

![Рис.9](images/TSel-zvonok.png)

Данные по звонкам коллтрекинга CallKeeper могут также отображаться в виде Конверсии, для этого необходимо предварительно создать соответствующую цель в Яндекс.Метрике с типом условия JavaScript-событие, идентификатор цели для звонков коллтрекинга calltracking_call_order или обратного звонка call.

![Рис.9](images/tsel.png)

Данная цель может быть использована для настройки автоматических стратегий, корректировки ставок в рекламных кампаниях Яндекс.Директа.

**Важно:** звонки, отправляемые в Яндекс.Метрику, могут обрабатываться внутри Яндекс.Метрики в течение 24 часов и не отображаться в отчетах до окончания обработки.
По вопросам, связанным с отправкой звонков в Яндекс.Метрику, пишите нам на i@callkeeper.ru или вашему персональному менеджеру. 


[Вернуться к оглавлению](#навигация)

[Вернуться на главную](/README.md/#documentation)
