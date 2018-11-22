# Описание интерфейса Room 
Интерфейс предназначен для работы с методами класса Room

## Реализация интерфейса 
* +add(Room:[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")) : int – функция добавления помещения в БД. Параметр «[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")» — помещение, которое необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления помещения из БД по заданному параметру;
* +save(Room:[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")) : bool – функция сохранения изменений. Параметр «[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")» — помещение, которое необходимо редактировать в БД;
* +getRoomById (Id : int) : [Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room") – функция, осуществляющая поиск помещения в БД по ID и возвращающая найденное помещение, если таковое имеется;
* +getRooms(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")> — функция, возвращающая список помещений с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getRoomContract(Id : int) : List<[Contract](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Contract.md "объект класса Contract")> -  возвращает список всех договоров помещения c заданными параметрами;
* +getProfitableRooms(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List <[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")> - функция, возвращающая список самых прибыльных помещений с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
