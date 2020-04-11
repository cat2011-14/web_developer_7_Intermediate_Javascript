# web_developer_7_Intermediate_Javascript

## Classes

JavaScript - это язык объектно-ориентированного программирования (ООП), который мы можем использовать для моделирования реальных объектов.

Классы - это инструмент, который разработчики используют для быстрого создания похожих объектов.

```
let halley = {
  _name: 'Halley',
  _behavior: 0,

  get name() {
    return this._name;
  },

  get behavior() {
    return this._behavior;
  },

  incrementBehavior() {
    this._behavior++;
  }
}
```
Как видите, классы - это отличный способ сократить время дублирования кода и время отладки

### Constructor
Хотя вы можете увидеть сходство между классом и синтаксисом объекта, существует один важный метод, который разделяет их. Это называется метод конструктора . JavaScript вызывает constructor()метод каждый раз, когда создает новый экземпляр класса.
```
class Dog {
  constructor(name) {
    this.name = name;
    this.behavior = 0;
  }
}
```

Экземпляр является объектом , который содержит имена свойств и методы класса, но с уникальными значениями свойств
```
class Dog {
  constructor(name) {
    this.name = name;
    this.behavior = 0;
  } 
}

const halley = new Dog('Halley'); // Create new Dog instance
console.log(halley.name); // Log the name value saved to halley
// Output: 'Halley'
```

### Methods
Синтаксис метода класса и метода получения такой же, как и для объектов, за исключением того, что вы не можете включать запятые между методами .
```
class Dog {
  constructor(name) {
    this._name = name;
    this._behavior = 0;
  }

  get name() {
    return this._name;
  }

  get behavior() {
    return this._behavior;
  }

  incrementBehavior() {
    this._behavior++;
  }
}
```

### Method Calls
