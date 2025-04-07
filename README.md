# UML

@startuml
left to right direction
Пользователь as fc
rectangle "Мобильное приложение" {
  usecase "Авторизация/Регистрация" as UC1
  usecase "Отправить сообщение" as UC2
  usecase "Обращение в техподдержку" as UC3
}
fc --> UC1
fc --> UC2
fc --> UC3

Администратор as adm
adm --> UC1
adm --> UC3

@enduml
