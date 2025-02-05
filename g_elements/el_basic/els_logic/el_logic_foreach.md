# Цикл ForEach

![](<../../../.gitbook/assets/image (100) (1) (1) (1) (1) (1) (1) (10) (168).png>)

![](<../../../.gitbook/assets/image (33).png>)

Элемент представляет собой цикл, перебирающий все значения выбранного массива.

Обратите внимание, что в свойствах есть два типа переменных - обычная и виртуальная. Для работы цикла требуется обязательно указать одну из них. По умолчанию используется виртуальная переменная item - она удаляется сразу после работы цикла и, таким образом, не занимает память. Обычную переменную рекомендуется использовать, если она потребуется в работе проекта в дальнейшем.

> *Описание общих свойств см. в разделе [**Работа с элементами**](https://docs.primo-rpa.ru/primo-rpa/primo-studio/process/elements)*

| Свойство     | Тип         | Описание                                                 |
| ------------ | ----------- | -------------------------------------------------------- |
| ***Процесс*** |          |                                                  |
| Массив\*     | ICollection | Массив, значения которого перебираются в цикле           |
| Виртуальная переменная\* |     | Переменная, хранящая значение текущей переменной массива. По умолчанию указана переменная item, которую возможно переименовать |
| Переменная | T           | Переменная, хранящая значение текущей переменной массива. В отличие от виртуальной, будет доступна в проекте даже после завершения работы цикла|
| Тип данных\* | String      | Тип данных итератора                                     |
| Индекс       | Int32       | Индекс текущей итерации                                  |

С работой цикла и массивами можно подробнее ознакомиться [в обучающем видео Студии](https://www.youtube.com/watch?v=TUIGnjNcI-Y&ab_channel=PrimoRPA).
