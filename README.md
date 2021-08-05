# План автоматизированного тестирования

## Перечень автоматизируемых сценариев:
1. Проверка двух видов входа на страницу для записи (совпадают ли страницы для входа через меню "Каталог курсов", так и через некоторый контент на главной странице)
2. Ввод данных с именем на русском языке и верным российским номером телефона
3. Ввод данных с именем на латинице и верным российским номером телефона
4. Ввод пустой формы
5. Ввод валидных данных с незаполненным полем с именем
6. Ввод валидных данных с незаполненным полем с телефоном

## Перечень используемых инструментов:
* Junit jupiter - основной инструмент тестирования
* Lombok - дает доступ к шаблонам кода
* Selenium - фреймворк для тестирования веб страниц
* Java Faker - с помощью него можно тестировать страницу с даннымми сгенерированных пользователей (вместо того, чтобы вносить данные вручную)
* Docker - инструмент виртуализации операцинной системы 
* Allure - инструмент для репортинга и более наглядного отображения результатов тестирования

## Перечень необходимых разрешений/данных/доступов:
* API
* Для генерации данных пользователей можно использовать Faker

## Перечень и описание возможных рисков при автоматизации:
* Возможность использования номеров телефонов и имен из любого региона мира

## Перечень необходимых специалистов для автоматизации:
Специалист по автоматизации со знанием инструментов Selenium, Faker, Lombok 

## Интервальная оценка с учётом рисков (в часах): 
* Подготовка общего плана тестирования - 1 час
* Написание тестов - 2 часа
