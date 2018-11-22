# Описание интерфейса Equipment 
Интерфейс предназначен для работы с методами класса Equipment 

## Реализация интерфейса 
* +add(Equipment:[Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment")) : int – функция добавления оборудования в БД. Параметр «[Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment")» — оборудование, которое необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления оборудования из БД по заданному параметру;
* +save(Equipment:[Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment")) : bool – функция сохранения изменений. Параметр «[Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment")» — оборудование, которое необходимо редактировать в БД;
* +getEquipmentById (Id : int) : [Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment") – функция, осуществляющая поиск оборудования в БД по ID и возвращающая найденное оборудования, если таковое имеется;
* +getAll(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Equipment](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Equipment.md "объект класса Equipment")> — функция, возвращающая список оборудований с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getEquipmentContract(Id : int) : List<[Contract](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Contract.md "объект класса Contract")> -  возвращает список всех договоров с оборудованием c заданными параметрами;
* +getEquipmentRoom(Id : int) : List<[Room](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Room.md "объект класса Room")> -  возвращает список всех помещений с оборудованием c заданными параметрами.
