Описание проекта
В этом проекте реализованно приложение для развёртывания процесов в Linux окружении. В проекте выднеляеться 3 основных части это - 
1) Сервир Агента который непосредственно запускаеться на самом сервере
2) Сервис контролера который умеет дублировать проект по разным машинам и также запускать их.
3) Сервис полезной нагрузки это сам сервис который мы запускаем в приложении.

# Сервис агента
## сервис агента имеет в себе функционал:
- Добаление приложения на сервер с помощью пути /add
- Удаление приложения с помощью пути /remove
- Запуск приложения с помощью пути /start
- Остановка приложения с помощью пути /stop
- загрузка приложения с помощью пути /upload
- Полученние статуса приложения с помощью пути /status
- Получение логов приложения с помощью пути /logs

# Сервис контролера
## сервис контролера имеет в себе функционал:
- Дублирование приложения на разные машины которые прописаны в конфигурации с помощью пути /add
- Узнавать статус всех машин из конфига с помощью пути /status
- Запускать приложение именно у себя с помощью пути /start
- и полностью удалять сервис со всех машин с помощью /remove