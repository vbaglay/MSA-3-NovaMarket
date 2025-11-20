| Этап | Тип события | Название события | Описание |
|------|-------------|------------------|-----------|
| Создание заказа | domain | OrderCreated | Покупатель создал заказ |
| Резервирование товара | domain | ReservationPlaced | Товар зарезервирован |
| Ошибка резервирования | failure | ReservationFailed | Недостаточно товара |
| Таймаут резервирования | timeout | ReservationTimeout | Резервирование истекло |
| Оплата начата | domain | PaymentStarted | Начата обработка платежа |
| Оплата успешна | domain | PaymentCompleted | Платеж успешно завершен |
| Ошибка оплаты | failure | PaymentFailed | Платеж отклонен |
| Таймаут оплаты | timeout | PaymentTimeout | Оплата не поступила |
| Отмена резервирования | compensation | ReservationCancelled | Освобождение товара |
| Возврат средств | compensation | RefundInitiated | Инициирован возврат |
| Заказ отменен | compensation | OrderCancelled | Заказ переведен в статус отмены |
| Готов к доставке | domain | OrderReadyForDelivery | Заказ готов к передаче в логистику |
| Доставка запланирована | domain | DeliveryScheduled | Логистика приняла заказ |
| Ошибка доставки | failure | DeliveryFailed | Логистика недоступна |
| Статус доставки обновлен | domain | DeliveryStatusUpdated | Изменен статус доставки |
| Заказ доставлен | domain | OrderDelivered | Заказ успешно доставлен |
| Уведомление отправлено | domain | NotificationSent | Пользователь уведомлен |