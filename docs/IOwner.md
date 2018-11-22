# Описание интерфейса Owner 
Интерфейс предназначен для работы с методами класса Owner 

## Реализация интерфейса 
* +add(Owner:[Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner")) : int – функция добавления владельца в БД. Параметр «[Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner")» — владелец, которого необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления владельца из БД по заданному парметру;
* +save(Owner:[Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner")) : bool – функция сохранения изменений. Параметр «[Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner")» — владелец, которого необходимо редактировать в БД;
* +getOwnerById (Id : int) : [Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner") –функция, осуществляющая поиск владельца в БД по ID и возвращающая найденного владельца, если таковой имеется;
* +getOwners(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Owner](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Owner.md "объект класса Owner")> — функция, возвращающая список владельцов с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getOwnerRoom(Id : int) : List<[Room](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Room.md "объект класса Room")> -  возвращает список всех помещений владельца c заданными параметрами;
* +getListOfDocuments(Id : int) : List <[Document](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Document.md "объект класса Document")> — возвращает список всех документов c заданными параметрами;
* +addDoc(Id_worker : int, Id_document : int) – функция добавления документа в БД;
* +delDoc(Id_worker : int, Id_document : int) - функция удаления документа из БД;
* +getDebt(Id : int) : [List<Payment>, List<Payment>](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Payment.md "объект класса Payment") – возвращает списки всех нужных платежей и произведенных оплат c заданными параметрами.
