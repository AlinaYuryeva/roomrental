# Описание интерфейса Contract 
Интерфейс предназначен для работы с методами класса Contract 

## Реализация интерфейса 
* +add(Contract:[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")) : int – функция добавления договора в БД. Параметр «[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")» — договор, который необходимо добавить в БД;
* +del(Id : int) : bool – функция удаления работника из БД по заданному параметру;
* +save(Contract:[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")) : bool – функция сохранения изменений. Параметр «[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")» — договор, который необходимо редактировать в БД;
* +getContractById (Id : int) : [Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract") – функция, осуществляющая поиск договора в БД по ID и возвращающая найденный договор, если таковой имеется;
* +getContracts(sorting : string, filtering : string, sortingA : string, count : int, page : int) : List <[Contract](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Contract.md "объект класса Contract")> — функция, возвращающая список договоров с заданными параметрами.
Параметры: 
  * sortintg: string — отвечает, по какому полю будет сортироваться список; 
  * sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы; 
  * filtering: string — отвечает за фильтрацию; 
  * count: int — отвечает, сколько элементов необходимо показать; 
  * page: int — отвечает, с какой страницы начинать поиск элементов.
* +getListOfDocuments(Id : int) : List <[Document](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Document.md "объект класса Document")> — возвращает список всех документов c заданными параметрами;
* +addDoc(Id_contract : int, Id_document : int) – функция добавления документа в БД;
* +delDoc(Id_contract : int, Id_document : int) - функция удаления документа из БД;
* +addEq(Id_contract : int, Id_equipment : int) – функция добавления оборудования из БД;
* +delEq(Id_contract : int, Id_equipment : int) - функция удаления оборудования из договора;
* +addSer(Id_contract : int, Id_service : int) – функция добавления услуги из БД;
* +delSer(Id_contract : int, Id_service : int) – функция удаления услуги из договора;
* +getContractEquipments(Id : int) : List<[Equipment](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Equipment.md "объект класса Equipment")> - возвращает список всех оборудований договора c заданными параметрами;
* +getContractPayment(Id : int) : List<[Payment](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Payment.md "объект класса Payment")> - возвращает список всех платежей договора c заданными параметрами;
* +getContractServices(Id : int) : List<[Service](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Service.md "объект класса Service")> - возвращает список всех услуг договора c заданными параметрами;
* +getDebt(Id : int) : [List<Payment>, List<Payment>](https://github.com/AlinaYuryeva/roomrental/blob/master/docs/Payment.md "объект класса Payment") – возвращает списки всех нужных платежей и произведенных оплат c заданными параметрами.