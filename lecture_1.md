# πLecture 1 : Abstraction, Hello! Python, Memory and Reassignment

## Contentsπ<a id="contents"></a>

* What is Data Science?[βοΈ](#0)
* Abstraction[βοΈ](#1)
* Hello! Python[βοΈ](#2)
* Memory and Reassignment[βοΈ](#3)

## What is Data Science?<a id="0"></a>[π](#contents)

> [κ°μ URLπ¬](https://youtu.be/xyTAi70RReQ)

**Data Science?**

* A-B-C : AI/Algorithm - Bigdata - Computing + D : Domain -> Application : λ°μ΄ν°μ μμ€κ° λ°μ
* Drawing useful **conclusions** from data using **computation**.
  * λΉλ°μ΄ν° μλμ΄κΈ°μ μ»΄ν¨ν°λ₯Ό μ μ¬μ©νλ κ²μ΄ μ€μν¨.
  * κ²°λ‘ μ μν΄ λ°μ΄ν°λ₯Ό μ΄ν΄νκΈ° μν΄ λ€μν μ κ³΅μ΄ μ ν¨ν¨.

**Computer Science?**

* Making computers do what you want to do **efficiently** (for your **productivity**)
* μ»΄ν¨ν°λ₯Ό μμ°λ κ²μ΄ μ€μν¨
* λ€μν μ’λ₯μ μ»΄ν¨ν°κ° λ΄κ° νκ³ μ νλ μΌμ ν μ μλλ‘ μμ μμ¬λ‘ λΆλ €λ¨Ήμ΄μΌ ν¨.
* μ»΄ν¨ν°κ° **ν¨μ¨μ μ΄μ΄μΌ** λμ **μμ°μ±**μ΄ μ¬λΌκ°

**Algorithms and Programs**

* **Logical** steps(recipe)
* Written in a **computer language **(instruction set)
* μ»΄ν¨ν°κ° λ°λΌ κ°μ μλ μλ²½ν λΌλ¦¬μ  κ΅¬μ‘°λ₯Ό μ¬νν΄μΌ ν¨.
* νλ‘κ·Έλ¨μ νΉμ ν language -> `Zero Ambiguity`λ₯Ό κ°μ§

## Abstraction<a id="1"></a>[π](#contents)

> [κ°μ URLπ¬](https://youtu.be/xyTAi70RReQ)

**How does a computer run a `Python` program?**

* μ΄μ μ νλ€κ³  κ°μ νμ!
  * νΈλ€μ μΈμ  μμ§μ΄λμ§? νλ¬μ μΈμ  λ°λμ§?
  * νμ¬λΌ, λ²μ€, νΈλ­, μνΌμΉ΄ λ± μ°¨μ μ’λ₯μ λ¬΄κ΄νκ² μ΄μ μ νλ λ°©λ²λ§ μλ©΄ λλ€.
  * μ΄μ μ νλ μΈν°νμ΄μ€λ§ μκ³  μμΌλ©΄ μ΄μ νλλ° λ¬Έμ κ° λμ§ μμ.

Driver do not need to know **implementation** details about a car to drive it

*  tire, wheel, engine, size, weight

They just need to deal with user **interfaces**, such as handle and pedals

* Once they know how to handle interfaces, they can drive all of various cars in the worls

**Abstraction** : The process of preserving information that is relevant in a given context, and forgetting information that is irrelevant in that context

* We cannot remember and focus on many things at a time...
* People with different expertise/interest can focus on their jobs without worrying about other part

* λ΄ μ½λμ κ΅¬νμ λνμΌμ μμμΌλ§ λ΄ μ½λλ₯Ό μ μ μμΌλ©΄ μλ¨. -> νμμ νλ€κ² λ§λ¦.
* Abstractionμ ν΅ν΄ μ μ²΄ μμ΄λμ΄λ₯Ό μμ μλλ‘ λ§λ€μ΄μΌ ν¨. -> Abstraction λ°©μμ ν λ‘ !

**Abstraction - Machine Learning**

If you don't understand, don't worry about it. - Andrew Ng

TensorFlow, pytorch // matlab(abstractionμ΄ λ³λ‘ μμ.)

**Abstraction - Mobile Phone**

* μ€λ§νΈν°μ κ²½μ°

  κ°€λ­μ, κ΅¬κΈ ν½μ, μ€μ€λ―Έ(Hardware) - `Android`(Operation System) - μΈμ€νκ·Έλ¨, μ€, λ·νλ¦­μ€, μ§λ©μΌ(Application)

**Abstraction - More General Computer**

* Application : μ€, λ‘μ€νΈμν¬, νμν¬μΈνΈ
* OS : window11
* H/W : λ€νΈμν¬, CPU, μ€νΌμΉ΄, λͺ¨λν° λ±λ±

μμ ν μ€κ³κ° λλμ΄ μμ.

**Abstraction - Thank you Operating System!**

* Operation system(e.g., MS Window, Linux, macOS) is the only program in the computer that's allowed **direct access** to the hardware
* If any other application program wants to interact with hardware (fetch data from storage, draw on the screen, find out what key was just pressed on the keyboard), it sends a **request** to the OS(**indirect access**)
* If you are not writing an OS,  you don't need to care about hardware but OS
  * Some smartphone Apps support either Android or iOS, not both of them
  * Once an app is ported on Android, it works for all different kinds of Android phone

**Abstraction - Thank you Interpreter!**

![image-20221025143751787](images/image-20221025143751787.png)

* OS is still too low and complex to directly program an application on...

  * If you are not a hardcore programmer

* Another layer for you, called **Interpreter**

  * If you write a program using Python, the interpreter takes your program, translate it into a language that OS understands

  ![image-20221025144341106](images/image-20221025144341106.png)

* Now you don't have to worry about OS too! Just write a program and it will run on variuos OSes! 

**Python Interpreter**

* Multiple ways of playing with Python
  * Execute a Python program that is saved in a file with `a.py` extension
    * The interpreter will execute **the whole program** in the file
* Execute a program called a **shell**, and type Python statements one at a time
  -> μμ μ¬μ©νλ©΄ κ·Έλκ·Έλ μΈν°νλ¦¬ν°κ° μ€νλ¨.
  * The interpreter will execute **each statement** when you type it
* Execute **jupyter notebook**, type and execute a group of Python statements
  * The interpreter will execute **the group of statements**
    -> κ·Έλ£Ήμ κ°μ§κ³  μΈν°νλ¦¬ν°κ° μ€νλμ΄ νΈνκ² μ¬μ©ν  μ μμ.

### Summary

* Abstraction - Interface and implementation
  * For now, it is OK to know only interfaces
  * To become a power user, you need to learn **low level system programming**!
* Operating system and application
* Python Interpreter

![image-20221025145201839](images/image-20221025145201839.png)

