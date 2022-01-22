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
