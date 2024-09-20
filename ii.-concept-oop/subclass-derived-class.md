---
description: >-
  คลาสย่อย (subclass) หรือคลาสที่สืบทอด (derived class)
  คือคลาสที่สืบทอดคุณสมบัติ (attributes) และเมธอด (methods) จากคลาสอื่น
  ซึ่งเรียกว่าคลาสแม่ (superclass) หรือคลาสฐาน (base class)
---

# Subclass / Derived Class

* `Dog` และ `Cat` เป็นคลาสย่อยที่สืบทอดจากคลาส `Animal`



**คุณสมบัติของคลาสย่อย:**

1. **การสืบทอด**: คลาสย่อยจะมีคุณสมบัติและฟังก์ชันที่ถูกกำหนดในคลาสแม่ โดยไม่ต้องเขียนใหม่
2. **การปรับแต่ง**: คลาสย่อยสามารถปรับแต่งหรือเขียนฟังก์ชันใหม่ที่เฉพาะเจาะจงสำหรับคลาสนั้นได้ เช่น การเขียนฟังก์ชัน `makeSound` ในคลาส `Dog` และ `Cat` เพื่อให้ส่งเสียงที่ต่างกัน
3. **การใช้ซ้ำ**: สามารถใช้ฟังก์ชันที่มาจากคลาสแม่ได้ โดยที่ไม่ต้องเขียนโค้ดซ้ำซ้อน

### Java

```java
class Dog extends Animal {
    void makeSound() {
        System.out.println("Bark");
    }
}

class Cat extends Animal {
    void makeSound() {
        System.out.println("Meow");
    }
}

```

### Python

```python
class Dog(Animal):
    def make_sound(self):
        print("Bark")

class Cat(Animal):
    def make_sound(self):
        print("Meow")

```

### C++

```cpp
class Dog : public Animal {
public:
    void makeSound() override {
        cout << "Bark" << endl;
    }
};

class Cat : public Animal {
public:
    void makeSound() override {
        cout << "Meow" << endl;
    }
};

```
