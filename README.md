# LastChaosBot

Для работы бота обход не требуется. Бот работает через чтение\запись памяти в процесс игры. Нажатие кнопок происходит через функции WinAPI. Бот может работать в свернутом режиме вместе с самой игрой.

![Screenshot 1](https://pp.userapi.com/c855124/v855124935/572e1/A8bf5yn2Eu8.jpg)
![Screenshot 2](https://pp.userapi.com/c855124/v855124935/572ea/LsVar79e3UE.jpg)

Что сейчас есть:
* Скорость атаки, скорость бега, радиус атаки ( последнее скорее всего работает неверно)
* ТП хак (не мапхак)
* Радар мобов, игроков и предметов
* Отслеживание характеристик персонажа
* Ведение статистики (опыт в час, ОУ в час)
* Подбирает предметы (настраивается)
* Умеет применять склилы (во время боя) и юзать бафы (по таймеру)
* Умеет убегать при обнаружении игрока или РБ (настраивается отдельно)
* Умеет возвращаться на исходную позицию при застревании в чем либо
* Настройка радиуса поиска мобов, радиуса работы бота (чтобы не убегать от исходной позиции)
* Имеется функция выбора только ближайших мобов (еще в режиме тестирования)

Чего нет, но хотелось бы добавить:
* Мапхак (телепорт через подмену НПЦ или пунктов меню НПЦ). Пробовал делать через CE, после подмены игра зависает. Если кто-то знает, * * возможен ли еще мапхак - буду благодарен
* Перемещение персонажа не через ТП. Возможно ли без инжекта dll или хука функциий игры заставить персонажа бежать в определенную точку?* Скиллхак (быстрый откат), хак на радиус подбора предметов

Бот написан на Python версии 3.6. Как запустить:
1. Установить Python 3.6.8. Обязательно добавить путь к папке установки в PATH в системных настройках.
2. Установить PIP (опция в установщике).
Желательно устанавливать в корень диска C и не допускать пробелов в названии папок.
3. Через PIP установить psutil, PyQT5 и pywin32.
4. Открыть CMD либо другую удобную вам консоль от имени Администратора.
5. Запустить через нее бота.
6. После запуска бота запустить саму игру.
7. Как только персонаж появится в мире нажать на большую кнопку.
8. Настроить, прийти на место кача или фарма, запустить.

* main.py - исходник самого бота
* ui.py - исходник интерфейса
* UI.ui - сам интерфейс, можно редактировать при помощи QDesigner
* Nksp.CT - таблица для CheatEngine
