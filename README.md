Граббер данных
=========

## Использование
Перед использованием сначала необходимо обновить автолоадер:
```
composer dump-autoload
```
Затем запустить сам импорт:
```
./parse.php
```

## Затраченное время
- composer, автолоадер, черновая структура проекта - 1ч
- Классы, структура, запросы - 3ч
- Парсинг документа - 3ч
- Доработки по структуре - 0,5ч
- Комментирование - 1
- Получение и парсинг изображений - 3ч

## Дополнителнительные сведения
`./parse.php` и `SiteParser\RuanRuBoardsParser` Пример парсер-скрипта на основе реализованных классов.
По задумке для каждого набора данных пишется свой класс-парсер.
За счёт использования интерфейсов мы добиваемся меньшей связности. Классы знают друг о друге ровно столько, сколько им положено для минимальной работы. Каждый класс выполняет лишь свою небольшую функцию
При разработке я старался следовать принципам SOLID.
В задании необходимо было НЕ использовать готовые библиотеки, а пользоваться стандартными средствами PHP и регулярными выражениями.