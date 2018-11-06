# Базы Данных

[Описание БД](http://msdn.microsoft.com/ru-ru/library/ms124438.aspx)

## Информация для подключения к серверу

Данная информация понадобится, чтобы подключиться к локальному серверу MS SQL Server, расположенному на территории университета ИТМО.

Адрес сервера: `192.168.10.72`

Логин: `student`

Пароль: `123654`

## Описание БД

* __Production__
    * Product 

        *Содержит продаваемые продукты или продукты, используемые в производстве.*
    
    * BillofMaterials
    
        *Список компонентов, используемых в производстве велосипедов и их комплектующих. ProductAssemblyID представляет родительский (или первичный) продукт, а ComponentID представляет его компоненты (или отдельные части), используемые при сборке первичного продукта. Например, сборка колеса содержит такие компоненты, как отражатели, обод, спицы, шину и камеру.*
    
* __Purchasing__
    * ProductVendor

        *Является таблицей перекрестных ссылок, в которой сопоставляются поставщики и поставляемые ими продукты для компании Adventure Works Cycles.*

    * Vendor

        *Содержит названия компаний, у которых Adventure Works Cycles покупает запчасти или другие товары.*

    * VendorContact

        *Таблица перекрестных ссылок, в которой сопоставляются компании-поставщики, ведущие коммерческую деятельность с торговыми сотрудниками компании Adventure Works Cycles, и их сотрудники. Например, покупатель Adventure Works Cycles свяжется с коммерческим представителем поставщика, чтобы приобрести комплектующие или продукцию.*
        
    * VendorAddress
        
        *Таблица перекрестных ссылок, в которой сопоставляются поставщики и их адреса. Поставщики могут иметь более одного адреса, например отдельные адреса для выставления счетов и доставки.*

* __Person__
    * Contact

        *Содержит список фамилий и другие сведения о каждом заказчике, сотруднике или поставщике. Например, заказчик (магазин) может указать торгового агента в качестве основного контактного лица своей компании и менеджера по продажам в качестве дополнительного контактного лица.*

    * Address
        
        *Содержит адреса всех заказчиков Adventure Works Cycles, поставщиков и работников. Заказчики и поставщики могут иметь несколько адресов. Например, заказчик может иметь разные адреса для выставления счетов и доставки.*

* __HumanResources__
    * Employee

        *Содержит сведения о работнике, такие как ИНН, должность и количество часов отпуска или количество отгулов. Имена работников хранятся в таблице Contact.*

* __Sales__
    * SalesOrderHeader

        *Содержит сведения об общем или родительском заказе на продажу. Конкретные продукты, связанные с заказом на продажу, хранятся в таблице SalesOrderDetail.*

    * SalesOrderDetail

        *Содержит отдельные продукты, связанные с определенным заказом на продажу. Заказ на продажу может содержать заказы на несколько продуктов. Общие или родительские сведения по каждому заказу на продажу хранятся в таблице SalesOrderHeader. Каждый заказанный продукт или потомок хранится в таблице SalesOrderDetail.*

    * SpecialOfferProduct

        *Таблица, в которой приведены скидки на различные виды (наименования) продукции.*

    * CreditCard
    
        *Содержит сведения о кредитной карте клиента, в частности номер карты и срок истечения.*
    
    * SalesPerson
    
        *Содержит текущие сведения о продажах для коммерческих представителей.*
    
    * Customer
    
        *Содержит текущие сведения о заказчике. Клиенты разбиты на категории по типам — частный потребитель или магазин розничной торговли.*
    
    * CustomerAdress
    
        *Сопоставляет заказчиков с их адресами. Например, заказчик может иметь разные адреса для выставления счетов и доставки.*
    
## Ссылки

* MS SQL Server [[скачать]](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

* SSMS [[скачать]](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms)

* AdventureWorks 2005 [[скачать]](http://msftdbprodsamples.codeplex.com/releases/view/4004)