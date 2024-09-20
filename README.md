---
description: การเขียนโปรแกรมเชิงวัตถุ (Object Orient Programming) ด้วยภาษา Java
---

# Java

<pre class="language-java"><code class="lang-java">class Animal{
    public Animal(){
        System.out.println("create animal");
    }
    public void finalize(){
        System.out.println("delete animal");
    }
    public void sound(){
        System.out.println("animal makes a sound");
    }
}
class Dog extends Animal{
    public Dog(){
        System.out.println("dog");
    }
    public void finalize(){
        System.out.println("delete dog");
    }
    @Override
    public void sound(){
        System.out.println("dog barks");
    }
}
class Cat extends Animal{
    public Cat(){
        System.out.println("cat");
    }
    public void finalize(){
        System.out.println("delete cat");
    }
    @Override
    public void sound(){
        System.out.println("cat meows");
    }
}
public class Main {
<strong>    public static void main(String[] args){
</strong>        Animal a = new Animal();
        Animal an = new Dog();
        Dog b = new Dog();
        Cat c = new Cat();
    
        an = c; //Polymorphic variable
        a.sound();
        an.sound();
        b.sound();
        c.sound();
    }
}
</code></pre>

### ผลลัพธ์ที่ได้จากการรันโค้ดข้างต้น&#x20;

```
create animal
create animal
dog
create animal
dog
create animal
cat
animal makes a sound
cat meows
dog barks
cat meows
```
