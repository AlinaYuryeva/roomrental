# Описание интерфейса Service 
Интерфейс предназначен для работы с методами класса Service

## Реализация интерфейса 
* +add(Service:[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")) : int – функция добавления услуги в БД. Параметр «[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")» — услуга, которую необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления услуги из БД по заданнному параметру;
* +save(Service:[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")) : bool – функция сохранения изменений. Параметр «[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")» — услуга, которую необходимо редактировать в БД;
* +getServiceById (Id : int) : [Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service") – функция, осуществляющая поиск услуги в БД по ID и возвращающая найденную услугу, если таковая имеется;
* +getAll(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")> — функция, возвращающая список услуг с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getServiceContract(Id : int) : List<[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")> -  возвращает список всех договоров с услугой c заданными параметрами;
* +getServiceRoom(Id : int) : List<[Room](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Room.md "объект класса Room")> -  возвращает список всех помещений с услугой c заданными параметрами.

