Most Wanted Online
==================

## Краткое описание сути проекта:
Модификация для игры Need For Speed: Most Wanted (2005), позволяющая множеству игроков играть свместно через сеть Интернет.

## Цель
Создание массовой многопользовательской гоночной платормы на основе существующей популярной игры ради тренировки.

## Конкуренты:
* NFS World
* GTA V
* Grid 2
* Forza Horizon
* Project CARS

## Сводная таблица сравнения 
| Проект | Стоимость лицензии (руб) | Минимальная поддеживаемая видеокарта
|--------|--------------------------|----------------
| NFS World | условно бесплатная | N/A (проект закрыт) |
| GTA V | 1500 | nVidia 9800 GT |
| Grid 2 | 700 | nVidia GTX220 |
| Forza Horizon | 3700 | nVidia 65ti |
| Project CARS | 719 | nVidia GTX 260 |

## Результаты проекта:
Реализовано в виде динамически подгружаемой библиотеки для десктопного приложения игры, а так же разработано сопутствующее серверное ПО и сайт для проверки состояния и статистики пользователей, регистрации пользователей.

## ~10-15 ключевых характеристик/свойств продукта. Должны быть достижимыми и проверяемыми
1. Требуемая ОС: Windows 7 или новее (клиент)
2. Системные требования не превышают требования ОС (требуется видеокарта)
3. Несколько территориально-распределённых официальных серверов (Россия, Бразилия, США)
4. Поддержка работы с частными игровыми серверами
5. Поддержжка публичного мониторинга количества игроков на серверах (онлайн-карта) на сайте
6. Ведение статистики по пользователям (время, проведённое в игре, скорость прохождения радаров, рейтинг гонок)
7. Расширенный набор автомобилей (по сравнению с оригинальной игрой)
8. Добавлена функция цикла "день/ночь", синхронизированного с сервером
9. Поддержка виртуальных соперников для совместных гонок
10. Большая физическая красная кнопка на официальных серверах, решающая все проблемы перезагрузкой

## Задачи проекта:
* Хранение данных о пользователях (учётная запись, список автомобилей, количество игровой валюты, данные рейтинга)
* Реализация сетевых соединений "Клиент-Сервер" и "Сервер-Суперсервер"
* Синхронизация положения автомобилей пользователей в реальном времени (допускается задержка до 1/18 секунды)
* Расчёт траффика и полицейских погонь на сервере

## Допущения и ограничения
* Копия самой игры не входит в поставку приложения, поскольку согласно ст. 146 УК РФ мы не имеем права распространять нелицензионное ПО.
* Ввиду недостаточной пропускной способности Интернет-соединения сервера, одновременное присутствие более 200 игроков на сервере может приводить к недостаточной производительности сервера, вплоть до отключения отдельных игроков из-за таймаута
* На данный момент модификация отключает механизм погонь и движение траффика в игре ввиду невозможности их синхронизации (исправлено в подготавливаемом релизе beta 2.0)
* Проект находится на стадии тестирования и может быть несовместим со сторонним ПО
* Текущая версия несовместима с Windows XP ввиду присутствия устаревшей сборки Discord RPC, неподдерживающей работу на этой ОС (исправлено в подготавливаемом релизе beta 2.0)
