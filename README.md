# Развертывание приложения
1. Установите докер
2. Разместите все папки со следующими сервисами приложения в едином каталоге (например c:/order services или ~/order services в случае linux):
- [Order persistence](https://github.com/temkarus0070/OrderPersistence)
- [Order Sender](https://github.com/temkarus0070/OrderSender)
- [Order Generator](https://github.com/temkarus0070/OrderGenerator)
- [Pay Service](https://github.com/temkarus0070/PayService)
- [Analytic order service](https://github.com/temkarus0070/analyticOrderService)
3. В корне используемого на предыдущем шаге каталога разместите docker-compose.yml из [этого репозитория](https://github.com/temkarus0070/orderServicesContainer)
3. Запустите докер
4. Через терминал или командную строку сделайте текущим каталогом каталог из пункта **2)**
5. Выполните команду docker compose up
6. Ожидайте пока загрузятся образы необходимые для приложения, такие как Kafka, Postgressql, JDK и т.д
7. Ожидайте запуска всех сервисов приложения и старта кафки.
8. Приложение готово к использованию. Все ресурсы 
9. В сервисах, принимающих веб-запросы от клиентов, для получения информации об используемых операциях, параметрах запроса и url адресов для доступа к ним можно использовать ** swagger ** по следующей url ** адрес сервиса:port/swagger-ui/index.html **
