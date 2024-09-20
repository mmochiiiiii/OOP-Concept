---
description: >-
  การสืบทอด (Inheritance) เป็นกลไกที่ทำให้คลาสย่อย (subclass)
  สามารถสืบทอดคุณสมบัติ (attributes) และพฤติกรรม (methods) จากคลาสแม่
  (superclass) ได้ ซึ่งช่วยให้เราสามารถใช้โค้ดที่มีอยู่แล้วโดยไม่ต้องเขียน
---

# Inheritance

คลาส `Dog` และ `Cat` สืบทอดเมธอด `sound()` จากคลาส `Animal` ซึ่งทำให้ทั้งสองคลาสมีพฤติกรรมในการทำเสียงที่สามารถปรับแต่งได้ตามต้องการ

### Java

```java
class Dog extends Animal {
    void sound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    void sound() {
        System.out.println("Meow");
    }
}
```

### Python

```python
class Dog(Animal):
    def sound(self):
        print("Bark")

class Cat(Animal):
    def sound(self):
        print("Meow")
```

### C++

```cpp
class Dog : public Animal {
public:
    void sound() override {
        cout << "Bark" << endl;
    }
};

class Cat : public Animal {
public:
    void sound() override {
        cout << "Meow" << endl;
    }
};
```
