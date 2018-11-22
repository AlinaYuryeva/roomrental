# Описание интерфейса Document 
Интерфейс предназначен для работы с методами класса Document

## Реализация интерфейса 
* +add(Document:[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")) : int – функция добавления договора в БД. Параметр «[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")» — договор, который необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления договора из БД по заданному параметру;
* +save(Document:[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")) : bool – функция сохранения изменений. Параметр «[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")» — договор, который необходимо редактировать в БД;
* +getDocumentById (Id : int) : [Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document") – функция, осуществляющая поиск документа в БД по ID и возвращающая найденный документ, если таковой имеется;
* +getDocuments(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Document](https://github.com/AlinaYuryeva/RoomRental/blob/master/docs/Document.md "объект класса Document")> — функция, возвращающая список документов с заданными параметрами. 
Параметры: 
  * sortintg: string – отвечает, по какому полю будет сортироваться список;
  * sortingA: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  * filtering: string — отвечает за фильтрацию;
  * count: int — отвечает, сколько элементов необходимо показать;
  * page: int — отвечает, с какой страницы начинать поиск элементов.
