## Практические задания по теме «Делегаты»

### Задача 2
Представим, что у вас есть приложение для управления задачами. В нем есть класс Task, который содержит информацию о задаче, такую как название, описание и статус (выполнена или нет). Класс TaskManager отвечает за создание, обновление и удаление задач. 

Вам нужно создать делегат, который позволяет другим классам подписываться на событие изменения статуса задачи. Задача будет считаться выполненной, если ее статус изменится на "выполнена". Напишите метод с именем "CompleteTask" в классе TaskManager. Этот метод должен принимать в качестве параметра объект Task и устанавливать его статус в "выполнена". Затем вызовите делегат, чтобы уведомить всех подписчиков о том, что задача была выполнена.

В другом классе, напишите метод с именем "TaskCompletedNotification", который будет вызываться при событии изменения статуса задачи. Этот метод должен принимать объект Task в качестве параметра и выводить сообщение о том, что задача выполнена.

Наконец, создайте экземпляр класса TaskManager и добавьте несколько задач в список. Затем подпишитесь на событие изменения статуса задачи, вызывая метод "TaskCompletedNotification" и добавьте его в делегат. Затем вызовите метод "CompleteTask" для одной из задач и убедитесь, что сообщение о выполнении задачи выводится на консоль.
