[Вопросы для собеседования](README.md)

+ [Что такое Session?](hibernate.md#Что-такое-Session?)
+ [Что такое SessionFactory?](hibernate.md#Что-такое-SessionFactory?)

## Что такое SessionFactory ? 

SessionFactory (org.hibernate.SessionFactory) — неизменяемый потокобезопасный объект с компилированным маппингом для одной базы данных. Необходимо инициализировать SessionFactory всего один раз. Экземпляр SessionFactory используется для получения объектов Session, которые используются для операций с базами данных.

## Что такое Session ? 

Session (org.hibernate.Session) — однопоточный короткоживущий объект, который предоставляет связь между объектами приложения и базой данных. Он оборачивает JDBC java.sql.Connection и работает как фабрика для org.hibernate.Transaction. Разработчик должен открывать сессию по необходимости и закрывать ее сразу после использования. Экземпляр Session является интерфейсом между кодом в java приложении и hibernate framework и предоставляет методы для операций CRUD.