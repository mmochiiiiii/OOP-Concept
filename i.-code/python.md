---
description: การเขียนโปรแกรมเชิงวัตถุ (Object Orient Programming) ด้วยภาษา Python
---

# Python

```python
class Animal:
    def __init__(self):
        print("create animal")

    def __del__(self):
        print("delete animal")

    def sound(self):
        print("animal makes a sound")

class Dog(Animal):
    def __init__(self):
        super().__init__()
        print("dog")

    def __del__(self):
        print("delete dog")

    def sound(self):
        print("dog barks")

class Cat(Animal):
    def __init__(self):
        super().__init__()
        print("cat")

    def __del__(self):
        print("delete cat")

    def sound(self):
        print("cat meows")

def main():
    a = Animal()
    an = Dog()
    b = Dog()
    c = Cat()

    an = c  # Polymorphic variable
    a.sound()
    an.sound()
    b.sound()
    c.sound()

if __name__ == "__main__":
    main()
```

### ผลลัพธ์ที่ได้จากการรันโค้ดข้างต้น&#x20;

```
create animal
create animal
dog
create animal
dog
create animal
cat
delete dog
animal makes a sound
cat meows
dog barks
cat meows
delete animal
delete dog
delete cat
```
