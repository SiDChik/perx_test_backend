Тестовое задание на Python-разработчика
==============

Нужно создать github репозиторий и в нем разместить приложение aiohttp. Python 3.6. в корне проекта run.py. Сервер должен считать арифметическую прогресию в очереди. При запуске стартует веб-сервер, у сервера есть два endpointa:
1. Поставить задачу в очередь. Параметры:
- count - количество элементов целочисленное (int)
- delta - дельта между элементами последовательности (float)
- start - Стартовое значение
- interval - интервал в секундах между итерациями (float)

2. Получить отсортированный список задач и статусы выполнения этих задач. Поля результата для каждой задачи:
- Номер в очереди
- Статус: В процессе/В очереди
- count
- delta
- start
- interval
- Текущее значение рассчета
- Дата старта задачи

--------

### Требования:
- Отработанные задачи стирать
- В качестве хранения данных использовать память
- Сервер запускается одним процессом
- Вычисление текущего значения должно высчитываться по интервалу, а не по формуле разницы времени и количеству итераций.
- Очередь стартует, как только в нее попадает задача
- 1 "воркер" выполняет только одну задачу
- Должна быть установка, сколько паралелльно запущено "воркеров"

В случае возникновения вопросов, дополнений, можно писать Тимлиду в телеграм - @SiDChik (Станислав)