
---

### **ДЛЯ РАЗРАБОТКИ ВАЖНА <mark style="background: #FF5582A6;">АРХИТЕКТУРА</mark>**

---

> Если вы думаете, что <mark style="background: #BBFABBA6;">хорошая</mark> архитектура - дорого, попробуйте <mark style="background: #BBFABBA6;">плохую</mark>

---
### История и принципы
- Архитектура программного обеспечения появилась в 80-х годах
- Основные принципы: <mark style="background: #ABF7F7A6;">абстракция</mark>, <mark style="background: #ABF7F7A6;">разграничение</mark> <mark style="background: #ABF7F7A6;">полномочий</mark>
- Архитектура включает выбор <mark style="background: #ABF7F7A6;">структурных элементов</mark> и <mark style="background: #ABF7F7A6;">их интерфейсов</mark>
---


Проблемы плохой архитектуры

- Плохая архитектура увеличивает время понимания кода и стоимость разработки.
- Хорошая архитектура удовлетворяет потребности пользователей и разработчиков.
- Независимость от фреймворков, пользовательского интерфейса, базы данных и внешних сервисов.

![[Чистая архитектура.png]]

Пример:
![[Пример архитектуры на классах.png]]

Модели в виде
```c#
class User {
	public int Id {get; set;}
	public string Name {get; set;}
	public int StatusId {get;set;}

	public virtual Status Status = new Status(); //многие к одному ТУТ
	public ICollection<Order> Orders = new List<Order>(); //один ко многим СЮДА
}
```

