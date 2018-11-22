# Описание интерфейса Worker 
Интерфейс предназначен для работы с методами класса Worker 

## Реализация интерфейса 
* +add(Worker:[Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker")) : int – функция добавления работника в БД. Параметр «[Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker")» — работник, которого необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления работника из БД по заданному параметру;
* +save(Worker:[Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker")) : bool – функция сохранения изменений. Параметр «[Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker")» — работник, которого необходимо редактировать в БД;
* +getWorkerById (Id : int) : [Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker") –функция, осуществляющая поиск работника в БД по ID и возвращающая найденного работника, если таковой имеется;
* +getWorkers(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Worker](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Worker.md "объект класса Worker")> — функция, возвращающая список работников с заданными параметрами. 
Параметры:
  * sortintg: string — отвечает, по какому полю будет сортироваться список; 
  * sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы; 
  * filtering: string — отвечает за фильтрацию; 
  * count: int — отвечает, сколько элементов необходимо показать; 
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getWorkerContracts(Id : int) : List<[Contract](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Contract.md "объект класса Contract")> -  возвращает список всех контрактов работника c заданными параметрами;
* +getListOfDocuments(Id : int) : List <[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")> — возвращает список всех документов c заданными параметрами;
* +addDoc(Id_worker : int, Id_document : int) – функция добавления документа в БД;
* +delDoc(Id_worker : int, Id_document : int) - функция удаления документа из БД.
