# **Аренда помещений**

Система предназначена для оперативного управления арендой недвижимости.
В рамках проекта автоматизируется:
* 1.	управление данными о торговых точках, предназначенных для аренды;
* 2.	управление данными о потенциальных клиентах;
* 3.	управление информацией о заключенных договорах, фиксируя данные о торговой точке и клиенте, а также сроке аренды;
* 4.	анализ статистики работы;
* 5.	ведение отчета и контроля выполненных работ;
* 6.	повышение эффективности работы предприятия.

## Диаграмма компонентов
![Alt-текст](https://pp.userapi.com/c852320/v852320293/4c083/xLFEiNesGYE.jpg "Диаграмма компонентов")

На данной диаграмме изображены все компоненты: клиентское приложение, работники, владельцы, клиенты, договоры, платежи, помещения, документы, услуги, оборудования. Эти компоненты взаимодействуют друг с другом с помощью интерфейсов. 
  
## Диаграмма размещений
![Alt-текст](https://pp.userapi.com/c852320/v852320293/4c076/T2yTGQgqaGo.jpg "Диаграмма размещения")

На диаграмме размещения изображены узлы выполнения программных компонентов, а также объектов. Показано, что клиентское приложение, установленное на компьютере пользователя взаимодействует с сервером, который содержит в себе базу данных.

## Диаграммы интерфейсов
![Alt-текст](https://pp.userapi.com/c852228/v852228695/50168/jburulpf69g.jpg "Диаграмма интерфейсов")
![Alt-текст](https://pp.userapi.com/c852228/v852228695/5017f/dMlLqPOTkqs.jpg "Диаграмма интерфейсов")
![Alt-текст](https://pp.userapi.com/c852228/v852228695/50189/QAq4g3s0CS4.jpg "Диаграмма интерфейсов")
Интерфейсы:
* [IWorker](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IWorker.md "Интерфейс IWorker")
* [IClient](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IClient.md "Интерфейс IClient")
* [IOwner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IOwner.md "Интерфейс IOwner")
* [IContract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IContract.md "Интерфейс IContract")
* [IRoom](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IRoom.md "Интерфейс IRoom")
* [IPayment](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IPayment.md "Интерфейс IPayment")
* [IDocument](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IDocument.md "Интерфейс IDocument")
* [IEquipment](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IEquipment.md "Интерфейс IEquipment")
* [IService](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/IService.md "Интерфейс IService")