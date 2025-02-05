# Настройка студии

Для вызова окна настроек студии, нужно нажать кнопку Настройки меню Файл.

![](<../../.gitbook/assets/image (668).png>)

Данное окно содержит настройки, сгруппированные по категориям:

* Общие: базовые настройки студии
  * Отладчик: настройка отладчика
  * Оформление: внешний вид студии
* Network
  * Reverse-Proxy: настройки перехвата трафика
  * Оркестратор: настройка подключения к Оркестратору
* Инструменты
  * Расширения: настройка расширений браузера
* Мобильные устройства
  * Android: настройки интеграции с устройствами Android

## Общие

В данной панели происходит настройка:

* Кол-во строк журнала: максимальное отображаемое кол-во строк в панели Консоль
* Автосохранение процессов: автоматическое сохранение всех открытых процессов во временные файлы
* Период: интервал между созданиями автосохраненных файлов
* Логировать в файл: сохранение журнала отладчика в файле
* Отображать окно приветствия – управляет демонстрацией начальным окном студии
* Режим без кода - использовать режим "Без кода" по умолчанию для новых элементов
* Открывать последние процессы - автоматически открывать последние открытые процессы проекта

### Отладчик

В данной панели происходит настройка функций отладчика:

* Тип отладчика: выбор типа отладчика – ROBOT (запуск отладки на реальном роботе) и SEQUENCE (запуск отладки без робота - экспериментальный)
* Закрывать робота: автоматическое закрытие робота по завершении процесса
* Отображать консоль робота: отображает консоль робота при отладке
* Сворачивать Студию: сворачивает студию при отладке
* Отображать окно консоли: отображает окно консоли при отладке
* Проверять синтаксис: автоматическая проверка синтаксиса
* Трассировка: включение возможности трассировки
* Писать общий журнал в файл: запись журнала работы робота в файл
* Писать пользовательский журнал: запись пользовательских событий работы робота в файл
* Период ожидания робота: предельный период ожидания старта робота при отладке (мс)
* Тип робота: x64 или x86&#x20;

### Оформление

* Тема: выбор цветовой палитры студии
* Язык: выбор языка интерфейса. После изменения потребуется перезапуск студии
* Отображать вертикальные заголовки: отображать вертикальные заголовки контейнеров последовательности
* Стиль главного меню: отображать главное меню как ленту, либо как панель (устаревшее)
* Последовательность
*
  * Высота дроппера
  * Отступы элемента
  * Отступы внутри контейнера

## Network

### Reverse-Proxy

Настройки работы с сетью перехватчика трафика:

* Порт: порт, используемый перехватчиком
* Авторегистрация, как системного proxy: при старте перехвата, перехватчик автоматически устанавливается в качестве Proxy-сервера системы
* Перехватывать SSL: признак перехвата и расшифровки пакетов SSL/TLS
* Перехватывать входящий трафик: признак перехвата ответов на запросы

### Оркестратор

Настройка подключения к оркестратору (не доступна для Community версии):

* Адрес сервера
* Логин
* Пароль

## Инструменты

### Расширения

Данное меню управляет установкой расширений браузеров.

![](<../../.gitbook/assets/image (700).png>)

####

{% content-ref url="plugin-install/" %}
[plugin-install](plugin-install/)
{% endcontent-ref %}

## Мобильные устройства

### Android

Настройки интеграции с мобильными устройствами на базе Android

* Путь к ADB: путь к папке установки Android Device Bridge
