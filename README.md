# optional
Некоторое подобие optional.

# Описание
+ Optional(const T& elem) - конструктор. Создает элемент со значением elem.  
+ Optional(T&& elem) - конструктор перемещения. Перемещает элемент со значением elem.  
+ Optional(const Optional& other) - конструктор копирования.  
+ Optional(Optional&& other) - перемещающий конструктор копирования.   
+ Optional& operator=(const T& elem) - оператор присваивания по значению.  
+ Optional& operator=(T&& elem) - перемещающий оператор присваивания по значению. 
+ Optional& operator=(const Optional& other) - оператор присваивания.  
+ Optional& operator=(Optional&& other) - перемещающий оператор присваивания.  
+ bool HasValue() const - возвращает is_initialized_ - инициализирован ли данный объект.  
+ T& Value() - возвращает значение.  
+ void Reset() - вызывает деструктор для хранящегося внутри объекта.  
