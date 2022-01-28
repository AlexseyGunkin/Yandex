# Yandex

## Навигация
* [Описание ](#Описание)
* [Подключение Яндекс.Метрики в личном кабинете CallKeeper](#Подключение-Яндекс.Метрики-в-личном-кабинете-CallKeeper)



## Описание

В кабинете ckct.ru во вкладке Аналитика мы отображаем данные, которые можно группировать по выбранным параметрам.
У нас есть возможность отображать на этой странице расходы на каналы. Эти расходы получаем из Яндекс Директ, доступ к которому открывает Яндекс Метрика.

## Подключение Яндекс.Метрики в личном кабинете CallKeeper

Для создания интеграции необходимо:

1. Зайти в свой личный кабинет на https://ckct.ru/ :
![Рис.1](images/LK_CT_1.jpg)
2. Перейти на вкладку аналитика в левой части экрана и в открывшейся вкладке выбрать в верхнем меню пункт интеграции:
![Рис.2](images/inter_1.jpg)
3. Нажать на кнопку Подключить новый аккаунт в окне доступные интеграции:
![Рис.4](images/add_akk_1.jpg)
4. Откроется окно авторизации Яндекс , где необходимо ввести данные аккаунта под которым вы хотите войти:
![Рис.4](images/login_1.jpg)
5. После этого откроется странница на который необходимо выбрать счетчики которые вы хотите добавить: 
![Рис.1](images/shetshik.png)
6. 


## Поздравляем! Ваши счетчики добавлены в аналитику ckct.ru

**Важная информация:**

* Счетчики обновляются ежедневно, в момент открытия страницы аналитики. 
* Вы можете отключать и включать подключенные счетчики с помощью соответствующего переключателя.
* Подключаясь к Яндекс Метрике, мы получаем их id кампании, название кампании и величину трат. По умолчанию матчатся utm_campaign, в которых есть id кампании.
Если же в utm_campaign отсутствует id кампании, данные не сматчатся в автоматическом режиме. В таком случае, если вы не хотите менять содержимое
utm_campaign, можно использовать другую метку. Вы можете обратиться к своему менеджеру с этим вопросом, и мы настроим забор данных из другой метки.
