# План автоматизированного тестирования
Ниже представлен план автоматизированного функционального компонентного тестирования при пролучении надлежашего разрешения и доступа (в будущем). Проверятся будут два вида входа на страницу для записи на курсы: через меню "Каталог курсов" и через некоторый контент на главной странице, а также заполнение формы отправки данных.

## Перечень автоматизируемых сценариев:
1. Проверка двух видов входа на страницу для записи (совпадают ли страницы для входа через меню "Каталог курсов", так и через некоторый контент на главной странице - ссылки "Нео для начинающих", раздела "Актуальные темы" - "Программирование")
2. Проверка заполнения формы отправки данных:
3.
*Позитивные сценарии*

* Ввод валидных данных с именем на русском языке и верным российским номером телефона 
* Ввод валидных данных с именем на латинице и верным российским номером телефона
* Ввод валидных данных зарегистрованного пользователя
* Ввод валидных данных незарегистрованного пользователя
* 
*Негативные сценарии*

* Ввод невалидных данных в разделе имени (знаков %, ?)
* Ввод невалидных данных в разделе email (знаков %, ?)
* Ввод невалидных данных в разделе телефон (знаков %, ?)
* Ввод пустой формы
* Ввод валидных данных с незаполненным полем с именем
* Ввод валидных данных с незаполненным полем с телефоном
* Ввод валидных данных с незаполненным полем с email

## Перечень используемых инструментов:
* Junit jupiter - основной инструмент тестирования
* Lombok - дает доступ к шаблонам кода
* Selenium - фреймворк для тестирования веб страниц (основа автоматизированного тестирования)
* Java Faker - с помощью него можно тестировать страницу с даннымми сгенерированных пользователей (вместо того, чтобы вносить данные вручную), нужен так как предполагается тестирования формы записи
* Docker - инструмент виртуализации операцинной системы - нужен для проверки работы в любой системе
* Allure - инструмент для репортинга и более наглядного отображения результатов тестирования - для упрощения анализа результатов
* Окружение:
Windows 10 64bit

Java 11.0.10

## Перечень необходимых разрешений/данных/доступов:
* Разрешения на проведения автоматированного тестирования
* API
* Для генерации данных пользователей можно использовать Faker

## Перечень и описание возможных рисков при автоматизации:
* Трудности с поиском CSS-локаторов на страницах сайта
* Риск изменения структуры страниц при тестировании

## Перечень необходимых специалистов для автоматизации:
Специалист по автоматизации со знанием инструментов Selenium, Faker, Lombok 

## Интервальная оценка с учётом рисков (в часах): 
* Подготовка общего плана тестирования - 3 часа
* Написание тестов - 8 часов
* Наступление рисков при тестировании - 5 часов
