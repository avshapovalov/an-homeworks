## Задача 1. Библиотека
### Описание

Иерархия работников библиотеки. Реализовать совмещение нескольких ролей в библиотеке в одном исполнителе через интерфейсы. Каждый объект в программе умеет определенный набор действий. Часто программист, создающий объект, не представляет все ситуации, в которых тот будет использоваться. Также программисту, использующему объект, часто неизвестны все его детали. Для передачи информации, что должен уметь объект используются интерфейсы.

Примером интерфейсов в нашей библиотеке может служить понятие роли на проекте. Каждая роль подразумевает набор определенных операций, которые должен “уметь” объект User в программе.

Создайте Иерархию “Пользователи библиотеки” со следующими интерфейсами:
* Читатель – берет и возвращает книги.
* Библиотекарь – заказывает книги.
* Поставщик книг – приносит книги в библиотеку.
* Администратор – находит и выдает книги и уведомляет о просрочках времени возврата.

Учтите, что интерфейсы могут “совмещаться” на User-ах. Юзеры могут взаимодействовать другс другом (например библиотекарь заказывает у поставщика). Сделайте 2-3 примера классов, реализующих эти интерфейсы (реализовывать сами методы не обязательно).

### Реализация:
1. Создайте 4 интерфейса: `Reader`, `Librarian`, `Supplier`, `Administrator`. Каждый из них должен содержать описанные выше методы, например у администратора должен быть метод `overdueNotification(Reader reader)`. Методы могут принимать в качестве параметра других user-ов, например читатель берет книги у администратора, библиотекарь заказывает у поставщика и т.д.

2. Создайте несколько классов, демонстрирующих использование интерфесов. В часности, продемонстрируйте совмещение, например поставщик, который может быть также и читателем, библиотекарь – администратором и т.д. Реализация методов, описанных в интерфейсах не обязательна, но желательно продемонстрировать, как методы должны вызываться на объектах.
