# Описание интерфейса Client
Интерфейс предназначен для работы с методами класса Client

## Реализация интерфейса 
* +add(Client:[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")) : int – функция добавления клиента в БД. Параметр «[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")» — клиент, которого необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления клиента из БД по заданному параметру;
* +save(Client:[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")) : bool – функция сохранения изменений. Параметр «[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")» — клиент, которого необходимо редактировать в БД;
* +getClientById (Id : int) : [Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")) –функция, осуществляющая поиск клиента в БД по ID и возвращающая найденного клиента, если таковой имеется;
* +getClients(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")> — функция, возвращающая список клиентов с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getClientContract(Id : int) : List<[Contract](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Contract.md "объект класса Contract")> -  возвращает список всех договоров клиента c заданными параметрами;
* +getListOfDocuments(Id : int) : List <[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")> — возвращает список всех документов c заданными параметрами;
* +addDoc(Id_worker : int, Id_document : int) – функция добавления документа в БД;
* +delDoc(Id_worker : int, Id_document : int) - функция удаления документа из БД;
* +getClientPayment (Id : int) : [List<Payment>, List<Payment>](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Payment.md "объект класса Payment") – возвращает списки всех нужных платежей и произведенных оплат c заданными параметрами;
* getProfitableClients(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List <[Client](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Client.md "объект класса Client")> - функция, возвращающая список самых прибыльных клиентов с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
