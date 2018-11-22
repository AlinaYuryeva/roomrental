# Описание интерфейса Payment 
Интерфейс предназначен для работы с методами класса Payment 

## Реализация интерфейса 
* +add(Payment:[Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment")) : int – функция добавления платежа в БД. Параметр «[Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment")» — платеж, который необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления платежа из БД по заданному параметру;
* +save(Payment:[Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment")) : bool – функция сохранения изменений. Параметр «[Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment")» — платеж, который необходимо редактировать в БД;
* +getPaymentById (Id : int) : [Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment") – функция, осуществляющая поиск платежа в БД по ID и возвращающая найденный платеж, если таковой имеется;
* +getPayments(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Payment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment")> — функция, возвращающая список платежей с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getProceeds(EndDate : DateTime, StartDate : DateTime) : float – функция, возвращающая суммарную выручку по заданным параметрам;
* +getProfitAndLoss(EndDate : DateTime, StartDate : DateTime) : float – функция, возвращающая суммарную прибыль по заданным параметрам.
