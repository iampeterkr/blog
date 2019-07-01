---
# layout : rchive
title: "Introduction to Classes"
permalink: /introduction-classes/
excerpt: "We learn about Classes Syntax."
# last_modified_at: 2019-02-28T09:00:00-04:00
redirect_from:
- /theme-setup/
toc: true
---
  
  
  
<hr style="border: solid 1px #dddddd ;">    

LESSON    

Classes are a crucial part of object-oriented programming (OOP). In this lesson, we'll explain what classes are, why they're important, and how to use them effectively.

**설명:** [ 학습방향 ]     
클래스는 객체지향의 끝판왕 이라고 말할수 있다.    
이 장에서는, 우리는 클래스가 무엇이며, 왜 중요하며, 어떻게 효과적으로 사용하는지를 학습한다.
{: .notice--info}     
    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 1. Why Use Classes?    

Python is an object-oriented programming language, which means it manipulates programming constructs called objects. You can think of an object as a single data structure that contains data as well as functions; the functions of an object are called its methods. For example, any time you call    
```python
len("Eric")
```    
Python is checking to see whether the string object you passed it has a length, and if it does, it returns the value associated with that attribute. When you call    

```python
my_dict.items()
```    
Python checks to see if my_dict has an items() method (which all dictionaries have) and executes that method if it finds it.    

But what makes "Eric" a string and my_dict a dictionary? The fact that they're instances of the str and dict classes, respectively. A class is just a way of organizing and producing objects with similar attributes and methods.   


<p style="page-break-before: always;"></p>
<br>



**설명:** [ Learn ]     
• Ch1. Why Use Classes? 에서는 클래스 정의에 대하여 학습한다.    
• Python 은 객체지향 프로그램이다.     
• 객체지향이란, 객체(objects)라고 불리는 것을 조작할수 있는 프로그램이다.    
• 우리는 함수(function)라는것을 배웠다. 이것도 하나의 객체(objects)이다.     
• 함수는 우리가 외부에서 arguments 로 입력값을 조절하며, 결과값을 구할 수 있었다.    
• 함수의 또다른 이름은 메서드(methods)라고 한다.    
• 이런 메서드들을 모아 놓은 것을 클래스라 한다.     
• 클래스를 함수 = 메서드 = 객체의 개념적 틀이라고 일단 생각하자.    
• 여기서는 여기까지 개념을 잡고, 더 자세한 내용은 다음 장에서 설명하겠다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor to the right.     
* We've defined our own **class**, Fruit, and created a lemon **instance**.    
* When you're ready, click Run to get started creating classes and objects of your own.     


**설명:** [ Instruction ]    
• Editor 화면의 소스를 분석해 보자.    
• 클래스 Fruit(object) 와, 인스탄스(instance) lemon 이 정의되어 있다.    
• Run을 클릭하면, 자신만의 클래스와 객체(objects) 만들어 진다. 
{: .notice--info}    



<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]    
• skip
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Fruit(object):
"""A class that makes various tasty fruits."""
  def __init__(self, name, color, flavor, poisonous):
    self.name = name
    self.color = color
    self.flavor = flavor
    self.poisonous = poisonous

  def description(self):
    print "I'm a %s %s and I taste %s." % (self.color, self.name, self.flavor)

  def is_edible(self):
    if not self.poisonous:
      print "Yep! I'm edible."
    else:
      print "Don't eat me! I am super poisonous."

lemon = Fruit("lemon", "yellow", "sour", False)

lemon.description()
lemon.is_edible()
```

**설명:** [ Solution ]     
• 클래스 Fruit(object) 가 정의되어 있다.    
• 클래스 Fruit 는 object 를 상속 받고 있다.    
• Object 상속의 개념은 추후에 설명할 것이다.    
• 클래스 Fruit(object) 에는 3개의 메소드가 정의되어 있다.   
• e.g. def `__init__():`,    
• e.g. def description(self):,     
• e.g. def is_edible(self):     
• 클래스 밖에는 lemon 이라는 객체가 만들어 진다.     
• 이 lemon 객체는 Fruit 클래스의 instance 를 가진다.    
• 객체 lemon을 통하여 Fruit 클래스의 description() 메서드를 사용한다.    
• 객체 lemon을 통하여 Fruit 클래스의 is_edible() 메서드를 사용한다.  
{: .notice--info}


**결과**     
``` 
I'm a yellow lemon and I taste sour.
Yep! I'm edible.
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 2. Class Syntax    

A basic class consists only of the `class` keyword, the name of the class, and the class from which the new class **inherits** in parentheses. (We'll get to inheritance soon.)     
For now, our classes will **inherit** from the object class, like so:    

```python
class NewClass(object):
# Class magic here
```    
This gives them the powers and abilities of a Python object.     
By convention, user-defined Python class names start with a capital letter.    




**설명:** [ Learn ]     
• Ch2. Class Syntax 에서는 클래스의 문법을 학습한다.         
• class 클래스 이름 (objects):    
• - class : 이 정의된 것이 클래스임을 알려줌.    
• - 클래스 이름 : 메서드들을 대표할수 있는 이름을 적어줌.    
• - (objects) : objects 의 기능을 상속(inherits) 받는다.    
• (objects) 라고 선언하면 Pythond object 의 기능을 활용할수 있게 해준다.    
• Python 은 클래스 이름을 쓸때, capital letter 방식으로 정의한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a class called `Animal` in the editor.     
* For now, in the body of your class, use the `pass` keyword. (pass doesn't do anything, but it's useful as a placeholder in areas of your code where Python expects an expression.)     


**설명:** [ Instruction ]    
• 클래스 Animal 을 작성하라.        
• 클래스 Animal 내부에 pass 키워드를 사용하라.    
• pass 는 추후에 설명하겠다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the example in the instructions as a guide!


**설명:** [ Hint ]     
• 상단의 클래스를 정의 한것을 참조하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
    pass

```

**설명:** [ Solution ]     
• 클래스 Animal 를 정의하였다.    
• 클래스 Animal 은 object 를 상속(inherit) 한다.     
• Animal 내부에 pass 키워드를 넣었다.
{: .notice--info}


**결과**     
``` 
#skip
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 3. Classier Classes    

We'd like our classes to do more than... well, nothing, so we'll have to replace our pass with something else.

You may have noticed in our example back in the first exercise that we started our class definition off with an odd-looking function: `__init__()`.     
This function is required for classes, and it's used to initialize the objects it creates. `__init__()` always takes at least one argument, self, that refers to the object being created.    
You can think of `__init__()` as the function that "boots up" each object the class creates.





**설명:** [ Learn ]     
• Ch3. Classier Classes 에서는 메서드 `__init__():` 를 학습한다.      
• 클래스 내부의 키워드 pass 자리에 어떤 기능들을 구현 하여야 한다.     
• 클래스 1장에서 클래스를 소개하면서 보여준 소스에서, `__init__()` 메서드를 보았다.    
• `__init__()` 는 클래스에서 반드시 필요한 메서드이다.    
• `__init__()` 는 클래스 객체가 생성될때, 초기화 하는데 사용된다.    
• `__init__()` 는 최소한 1개의 argument self 를 가진다.    
• `__init__()` 는 객체가 생성될 때마다 실행되는 함수이자 메서드이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Remove the pass statement in your class definition, then go ahead and define an `__init__()` function for your Animal class.     
* Pass it the argument self for now; we'll explain how this works in greater detail in the next section.     
* Finally, put the pass into the body of the `__init__()` definition, since it will expect an indented block.


<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• 키워드 pass 를 제거하고, 그자리에 `__init__()` 를 정의하라.    
• `__init__()` 는 기본적으로 arguments 인 self 를 가진다.    
• `__init__()` 내부에 키워드 pass 를 넣어라.    
•  단, 들여쓰기(indented block)를 주의하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your `__init__()` function should look something like this:    

```python
def __init__(self):
  pass
```

**설명:** [ Hint ]     
• `__init__(self)` 사용법을 참조하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
    def __init__(self):
      pass
```

**설명:** [ Solution ]     
• 클래스 Animal(object) 를 정의한다.    
• 내부 메서드 `__init__(self)` 를 선언한다.     
• 그안에 pass 키워드를 입력한다. 
{: .notice--info}



**결과** 
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 4. Let's Not Get Too Selfish    

Excellent! Let's make one more tweak to our class definition, then go ahead and instantiate (create) our first object.

So far, `__init__()` only takes one parameter: `self`. This is a Python convention; there's nothing magic about the word `self`. However, it's overwhelmingly common to use `self` as the first parameter in `__init__()`, so you should do this so that other people will understand your code.

The part that is magic is the fact that `self` is the first parameter passed to `__init__()`. Python will use the first parameter that `__init__()` receives to refer to the object being created; this is why it's often called `self`, since this parameter gives the object being created its identity.



**설명:** [ Learn ]    
• Ch4. Let's Not Get Too Selfish 에서는 self 에 관하여 학습한다.     
• 메서드 `__inti__()` 는 self 를 매개변수를 가진다. 이것은 Python 약속이다.    
• self 가 특별한 것은 없지만, 무조건 `__inti__()` 의 첫번째 매개변수로 사용된다.    
• 클래스가 호출되면, 자동으로 `__init__(slef)` 가 호출된다.     
• 호출될때, 자기 자신을 호출하기에, self 라고 부른다.    
• self 가 호출 되는것은 이 객체의 정체성(누구 것인지)를 알게 해준다.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's do two things in the editor:

* Pass `__init__()` a second parameter, `name`.    

* In the body of `__init__()`, let the function know that `name` refers to the created object's `name` by typing `self.name = name.` (This will become crystal clear in the next section.)

<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• 메서드 `__init__(self)` 의 두번째 매개변수(parameter)에 변수 name 을 넣자.    
• 메서드 `__init__(self, name)` 의 내부에 `self.name = name` 라고 만든다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

```python    
class Animal(object):
  def __init__(self, name):
    # Set the name parameter here!
```

**설명:** [ Hint ]     
• 메서드 `__init__(self, name)` 에 두번째 매개변수에 변수 name 을 정의하자.    
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
  def __init__(self, name):
    self.name = name
```

**설명:** [ Solution ]     
• 클래스 Animal 안, 메서드 `def __init__(self, name):` 를 정의한다.    
• 변수 `self.name = name` 이라고 정의한다.     
• 이 뜻은 매개변수 name 의 값을 self.name 에 저장한다는 뜻이다.
{: .notice--info}



**결과**     
``` 
#skip
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 5. Instantiating Your First Object    

Perfect! Now we're ready to start creating objects.

We can access attributes of our objects using dot notation. Here's how it works:     
<br>
```python

class Square(object):
  def __init__(self):
    self.sides = 4

my_shape = Square()
print my_shape.sides 
# my_shape. 찍는순간 __init__(self)가 호출된다.

```
<br>

* First we create a class named Square with an attribute sides.    
* Outside the class definition, we create a new instance of Square named my_shape and access that attribute using my_shape.sides.    


**설명:** [ Learn ]      
• Ch5. Instantiating Your First Object 에서는 Instance 를 학습한다.    
• 클래스의 기본은 만들어 졌다. 우리는 Instance 를 만들수 있다.     
• ( . ) 을 사용하여 우리는 객체의 속성에 접근할 수 있다.    
• 객체 my_shape 를 만드는 방법은 다음과 같다.    
• e.g. my_shape = Square()    
• 생성된 객체(Object) my_shape 는 클래스 Square() 의 속성을 그대로 사용할 수 있다.    
• 객체 my_shapes 를 클래스 Square() 의 내부 속성을 사용할려면, 다음과 같다.    
• my_shape. 이라고 ( . )을 찍는 순간 클래스의 `__init__(self)` 가 자동 호출된다.    
• my_shape.sides 는 `__init__(self)` 의 self.sides 에 접근할 수 있다.    
• self.sides = 4 이기에,     
• print my_shape.sides 는 4 가 출력된다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Outside the `Animal` class definition, create a variable named `zebra` and set it equal to `Animal("Jeffrey")`.

* Then print out zebra's name.     


**설명:** [ Instruction ]    
• 클래스 Animal 바깥에, 변수 zebra 를 생성하라.    
• zebra = Animal("Jeffrey") 선언하라.(객체 생성)      
• 변수 zebra 의 이름을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can create a new `Animal` object named "Jeffrey" like this:

```python

zebra = Animal("Jeffrey")

```
You can print out "Jeffrey"'s name like this:

```python

print zebra.name

```


**설명:** [ Hint ]     
• 클래스 Animal 를 사용하는 객체(object) zebra 를 생성한다.    
• zebra.name 을 호출하면, 클래스 Animal 의 name 에 있는 내용이 출력된다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
  def __init__(self, name):
    self.name = name
  
zebra = Animal("Jeffrey")

print zebra.name
```

**설명:** [ Solution ]     
• 클래스 Animal 을 정의한다.     
• 클래스 Animal 은 Object 를 상속한다.    
• 클래스 Animal 은 메서드 `__init__(self, name):` 을 가진다.    
• 이 메서드는 입력받은 name 을 self.name 에 저장한다.    
• 객체 zebra 를 다음과 같이 생성한다.    
• e.g. zebra = Animal("Jeffrey")    
• 클래스 Animal 을 instance 하는 객체 zebra 를 생성한다.   
• 클래스 Animal() 의 파라메터에 값 "Jeffrey" 를 넣는다.    
• 변수 name 에는 "Jeffrey" 가 넘겨진다.     
• 객체 zebra 는 클래스 Aniaml 의 속성을 그대로 가지고 있다.    
• zebra. 하는 순간 클래스 Animal()의 `__init__(self)` 가 호출된다.    
• zebra.name 은 클래스 Animal 의 name 이 출력된다.
{: .notice--info}



**결과**     
``` 
Jeffrey
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 6. More on __init__() and self    

Now that you're starting to understand how classes and objects work, it's worth delving a bit more into `__init__()` and `self`. They can be confusing!

As mentioned, you can think of `__init__()` as the method that "boots up" a class' instance object: the init bit is short for "initialize."

The first argument `__init__()` gets is used to refer to the instance object, and by convention, that argument is called `self`. If you add additional arguments—for instance, a `name` and `age` for your animal—setting each of those equal to `self.name` and `self.age` in the body of `__init__()` will make it so that when you create an instance object of your `Animal` class, you need to give each instance a `name` and an `age`, and those will be associated with the particular instance you create.



**설명:** [ Learn ]     
• Ch6. More on `__init__()` and self 에서는 함수 init 와 self 를 추가 학습한다.    
• 객체를 생성할때, 함수 `__init__(self)` 가 자동 호출된다.     
• 함수 `__init__` 에는 self 외에도 name, age 매개 변수를 추가할 수 있다.    
• 함수 `__init__()` 이 호출되면 내부에는 self.name, self.age 가 만들어진다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the examples in the editor.     
* See how `__init__()` "boots up" each object to expect a `name` and an `age`, then uses `self.name` and `self.age` to assign those names and ages to each object?     
* Add a third attribute, `is_hungry` to `__init__()`, and click Run to see the results.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• Editor 화면에서 함수 `__init__()` 이 어떻게 기동 되는지 확인하라.    
• 매개변수 name , age 가 어떻게 self.name, self.age 로 할당되는지도 확인하라.    
• 함수 `__init__()` 에 is_hungry 를 세번째 매개변수로 추가 하여라.    
• 실행시켜 보아라. 그리고 결과를 지켜보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your code should look something like this:    

```python
def __init__(self, name, age, is_hungry)
  self.name = name
  self.age = age
  self.is_hungry = is_hungry
```


**설명:** [ Hint ]     
• 매개변수로 is_hungry 를 세번째 매개변수로 추가한다.     
• 추가한 매개변수 is_hungry 를 다음과 같이 정의한다.    
• e.g. self.is_hungry = is_hungry
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
# Class definition
class Animal(object):
  """Makes cute animals."""
  # For initializing our instance objects
  def __init__(self, name, age, is_hungry):
    self.name = name
    self.age = age
    self.is_hungry = is_hungry
```
<p style="page-break-before: always;"></p>
<br>

```python
# Note that self is only used in the __init__()
# function definition; we don't need to pass it
# to our instance objects.

zebra = Animal("Jeffrey", 2, True)
giraffe = Animal("Bruce", 1, False)
panda = Animal("Chad", 7, True)

print zebra.name, zebra.age, zebra.is_hungry
print giraffe.name, giraffe.age, giraffe.is_hungry
print panda.name, panda.age, panda.is_hungry

```

**설명:** [ Solution ]     
• 클래스 Animal 의 함수 `__init__` 에 매개변수 is_hungry 를 추가 하였다.    
• e.g. `def __init__(self, name, age, is_hungry):`    
• 함수 `__init__` 에 매개변수 is_hungry 를 할당 하였다.    
• e.g. self.is_hungry = is_hungry    
• 객체, zebra, giraffe, panda 를 생성할때, 3 번째 매개변수 값도 지정 하였다.
{: .notice--info}



**결과**     
``` 
Jeffrey 2 True
Bruce 1 False
Chad 7 True
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 7. Class Scope    

Another important aspect of Python classes is **scope**. The **scope of a variable** is the **context** in which it's visible to the program.

It may surprise you to learn that not all variables are accessible to all parts of a Python program at all times. When dealing with classes, you can have variables that are available everywhere (global variables), variables that are only available to members of a certain class (member variables), and variables that are only available to particular instances of a class (instance variables).

The same goes for functions: some are available everywhere, some are only available to members of a certain class, and still others are only available to particular instance objects.


**설명:** [ Learn ]    
• Ch7. Class Scope 에서는 클래스의 변수 주기를 학습한다.    
• 클래스에서 중요한게 변수의 주기(scope)이다.      
• 우리는 변수는 한번 생성되면 계속 접속 or 사용할수 있다고 생각한다.      
• 클래스 변수에는 3 종류가 있다.    
1 . 전역변수(global variables) : 어디서든 접근 가능    
2 . 클래스 변수(member variables) : 클래스 멤버만 접근 가능    
3 . 인스탄스 변수(Instance variables) : 클래스의 객체만 접근 가능 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.     
* Note that each individual animal gets its own `name` and `age` (since they're all initialized individually), but they all have access to the member variable `is_alive`, since they're all members of the `Animal` class.     
* Click Run to see the output!

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• Editor 안의 코드를 확인하라.        
• 클래스에서 변수 name, age 는 instance 변수 이다.        
• 클래스에서 변수 is_alive 는 클래스 변수 이다.     
• Run 실행시켜, 결과를 확인하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]     
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
    """Makes cute animals."""
    # class variables
    is_alive = True 
    def __init__(self, name, age):
      # instance variables
      self.name = name
      self.age = age

zebra = Animal("Jeffrey", 2)
giraffe = Animal("Bruce", 1)
panda = Animal("Chad", 7)

print zebra.name, zebra.age, zebra.is_alive
print giraffe.name, giraffe.age, giraffe.is_alive
print panda.name, panda.age, panda.is_alive

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 변수 is_alive 는 클래스 변수이다.    
• 변수 name, age 는 instance 변수이다. 
{: .notice--info}



**결과**     
```
Jeffrey 2 True
Bruce 1 True
Chad 7 True
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 8. A Methodical Approach    

When a class has its own functions, those functions are called **methods**. You've already seen one such method: `__init__()`. But you can also define your own methods!

<br>

**설명:** [ Learn ]    
• Ch8. A Methodical Approach 에서는 메서드를 학습한다.     
• 클래스가 가지고 있는 함수를 메서드(method) 라고 부른다.    
• 함수 `__init__()` 도 클래스의 메서드 이다.  
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add a method, `description`, to your `Animal` class.     
* Using two separate print statements, it should print out the `name` and `age` of the animal it's called on.     
* Then, create an instance of Animal, `hippo` (with whatever name and age you like), and call its `description` method. 

<br>

**설명:** [ Instruction ]    
• Animal 클래스에 메서드 description() 를 추가하라.     
• 메서드 description() 는 동물의 이름(name)과 나이(age)를 출력(print)한다.    
• Animal 클래스의 instance 를 가진 hippo 를 작성하라.     
• e.g. hippo = Animal()       
• 그 객체(object) hippo 의 메서드(method)인 description() 를 호출하라.  
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember to pass `self` as an argument to `description`.     
* Otherwise, printing `self.name` and `self.age` won't work, since Python won't know which `self` (that is, which object) you're talking about!    
* Your method should look something like this:    

```python
def description(self):
    print self.name
    print self.age
```      
* After that, all you need to do is create a `hippo` and call its description method with `hippo.description()`!    


**설명:** [ Hint ]     
• 메서드 description(self) 은 self parameter 가 있어야 한다.     
• 메서드 description() 가 호출되면, name 과 age 가 출력된다.    
• 생성된 객체 hippo.description() 으로 호출한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Animal(object):
    """Makes cute animals."""
    is_alive = True
    def __init__(self, name, age):
      self.name = name
      self.age = age
    # Add your method here!
    def description(self):
      print self.name
      print self.age
      
hippo = Animal("Anderson", 36)
hippo.description()
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 클래스 Animal 내부에 메서드 description(self) 를 만들었다.    
• 메서드 description(self) 는 name 과 age 를 출력한다.    
• 클래스 Animal("Anderson", 36) 을 instance 하는 object(객체) hippo 를 생성한다.    
• e.g. hippo = Animal("Anderson", 36)    
• object(객체) hippo 를 이용하여, 메서드 description() 을 호출한다.    
• e.g. hippo.description()
{: .notice--info}



**결과**     
``` 
Anderson
36
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 9. They're Multiplying!    

A class can have any number of **member variables**. These are variables that are available to all members of a class.    
```python
hippo = Animal("Jake", 12)
cat = Animal("Boots", 3)
print hippo.is_alive
hippo.is_alive = False
print hippo.is_alive
print cat.is_alive
```    
In the example above, we create **two instances** of an Animal.
Then we print out True, the default value stored in hippo's `is_alive` member variable.    
Next, we set that to False and print it out to make sure.
Finally, we print out True, the value stored in cat's is_alive member variable. We only changed the variable in hippo, not in cat.
Let's add another member variable to Animal.



**설명:** [ Learn ]     
• Ch9. They're Multiplying! 에서는 객체 생성 및 호출을 학습한다.       
• 클래스 Animal 의 instance 를 가진 2개의 object(객체) hippo, cat 을 만든다.   
• 객체 member 변수(클래스 변수) hippo.is_alive 를 호출 후, 출력한다.    
• 객체 변수 hippo.is_alive 값을 False 로 변경한다.    
• hippo.is_alive 를 출력한다.    
• 객체 cat.is_alive 를 호출 후, 출력한다.     
• 클래스 변수(member variables) is_alive 가 어떻게 동작되는지 생각해 본다.      
• 각각의 클래스변수(member variables) 가 객체별로 따로 관리된다.    
• 다른 객체(object)에 영향을 주지 않는다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* After line 3, add a second member variable called `health` that contains the string "good".

* Then, create two new Animals: `sloth` and `ocelot`. (Give them whatever names and ages you like.)

* Finally, on three separate lines, print out the `health` of your `hippo`, `sloth`, and `ocelot`.


**설명:** [ Instruction ]    
• 라인 3 에서, 2 번째 클래스(member) 변수 health 를 추가한다.    
• 클래스 변수 health = "good" 라고 할당한다.   
• 클래스 Animals 의 instance 를 가지는 sloth, ocelot 를 생성한다.    
• 객체(object) sloth, ocelot 에 이름과, 나이는 적당히 넣어라.    
• 객체 hippo, sloth, ocelot 의 health 를 각 라인에서 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You can add your member variable right under `is_alive`, like so:    

```python
is_alive = True
health   = "good"
```    

* You can print out your hippo's `health` with    

```python
print hippo.health
```


**설명:** [ Hint ]     
• 클래스(member) 변수 is_alive 밑에 클래스 변수 health 를 추가한다.     
• 객체(object) hippo.health 호출후 출력한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
class Animal(object):
    """Makes cute animals."""
    is_alive = True
    health = "good"
    def __init__(self, name, age):
      self.name = name
      self.age = age
    # Add your method here!
    def description(self):
      print self.name
      print self.age
  
hippo = Animal('Anderson', 36)
sloth = Animal('Dale', 15)
ocelot = Animal('Fuzzy', 7)

print hippo.health
print sloth.health
print ocelot.health
```

**설명:** [ Solution ]     
• 클래스 Animal에 클래스(member) 변수 health = "good" 를 추가한다.     
• 클래스 Animal의 instance 인 객체 hippo, sloth, ocelot 를 생성한다.    
• 객체 각각의 health 값을 호출 후, 출력한다. 
{: .notice--info}



**결과**     
``` 
good
good
good
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 10. It's Not All Animals and Fruits     

Classes like `Animal` and `Fruit` make it easy to understand the concepts of **classes** and **instances**, but you probably won't see many `zebras` or `lemons` in real-world programs.

However, classes and objects are often used to model real-world objects. The code in the editor is a more realistic demonstration of the kind of classes and objects you might find in commercial software. Here we have a basic `ShoppingCart` class for creating shopping cart objects for website customers; though basic, it's similar to what you'd see in a real program.

<br>

**설명:** [ Learn ]     
• Ch10. It's Not All Animals and Fruits 에서는 클래스를 실습한다.    
• 실전에서 클래스, 객체, 인스탄스가 어떻게 사용되는지를 쇼핑몰 카트를 만들어 보면서 이해하자.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create an **instance** of `ShoppingCart` called `my_cart`.     
* Initialize it with any values you like, then use the `add_item` method to add an item to your cart. 

<br>

**설명:** [ Instruction ]    
• 클래스 ShoppingCart의 instance 인 객체 my_cart 를 작성하라.    
• 메서드 add_item() 의 parameter 인 product, price 에 자신이 좋아하는 값을 넣어라.    
• 객체(object) my_cart 의 메서드 add_item() 을 통하여 product 와 price 를 추가하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Since the `ShoppingCart` class has an `__init__()` method that takes a customer `name`, I'd create `my_cart` like so:     

```python
my_cart = ShoppingCart("Eric")
```     

* Calling the `add_item()` method might then be:     

```python
my_cart.add_item("Ukelele", 10)
```


**설명:** [ Hint ]     
• 클래스 ShoppingCart 의 instance 인 my_cart 를 생성한다.    
• 이때, parameter 를 *Eric* 을 넣는다.    
• 객체(object) my_cart 에서 add_item() 메서드를 호출한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class ShoppingCart(object):
    """Creates shopping cart objects
    for users of our fine website."""

    def __init__(self, customer_name):
      self.customer_name = customer_name
      self.items_in_cart = {}

    def add_item(self, product, price):
      """Add product to the cart."""
      if not product in self.items_in_cart:
        self.items_in_cart[product] = price
        print product + " added."
      else:
        print product + " is already in the cart."

```
<p style="page-break-before: always;"></p>
<br>

```python    
def remove_item(self, product):
  """Remove product from the cart."""
  if product in self.items_in_cart:
    del self.items_in_cart[product]
    print product + " removed."
  else:
    print product + " is not in the cart."

my_cart = ShoppingCart("Eric")
my_cart.add_item("Ukelele", 10)
```

**설명:** [ Solution ]     
• 클래스 ShoopingCart("Eric") 의 instance 인 객체 my_cart 를 생성한다.    
• e.g. my_cart = ShoppingCart("Eric")    
• 객체(object) my_cart 의 메서드인 add_item("Ukelele", 10) 을 호출한다.    
• e.g. my_cart.add_item("Ukelele", 10)
{: .notice--info}



**결과**     
``` 
Ukelele added.
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 11. Warning: Here Be Dragons    

**Inheritance** is a tricky concept, so let's go through it step by step.

Inheritance is the process by which one class takes on the attributes and methods of another, and it's used to express an *is-a* relationship. For example, a Panda is a bear, so a Panda class could inherit from a Bear class. However, a Toyota is not a Tractor, so it shouldn't inherit from the Tractor class (even if they have a lot of attributes and methods in common). Instead, both Toyota and Tractor could ultimately inherit from the same Vehicle class. 



**설명:** [ Learn ]     
• Ch11. Warning: Here Be Dragons 에서는 Inheritance(상속) 을 학습한다.    
• Inheritance(상속) 에 대해서 배워보자.    
• Q1. 클래스 Panda 는 클래스 Bear 의 일부분 이다. 동의 하는가?    
• Q2. 클래스 Toyota 는 클래스 Tractor 의 일부분 이다. 동의 하는가?    
• Q3. 클래스 Toyota 는 클래스 Vehicle 의 일부분 이다. 동의 하는가?    
• Q4. 클래스 Tractor 는 클래스 Vehicle 의 일부분 이다. 동의 하는가?    
• 위 에서, Q2는 동의 되지 않는다. Toyota 는 Tractor 의 개념적 하위가 될 수 없다.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.    
* We've defined a class, `Customer`, as well as a `ReturningCustomer` class that inherits from `Customer`.     
* Note that we don't define the `display_cart` method in the body of `ReturningCustomer`, but it will still have access to that method via **inheritance**.     
* Click Run to see for yourself! 

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Instruction ]    
• Editor 화면에 있는 Code 를 살펴보자.    
• 클래스 Customer 가 정의되어 있다.    
• 클래스 ReturningCustomer 가 클래스 Customer 를 inheritance(상속) 하고 있다.    
• 주) 클래스 ReturningCustomer 내부에, 메소드 display_cart() 를 정의하지 않는다.    
• Run 실행하여, 결과를 살펴보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* skip


**설명:** [ Hint ]     
• skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Customer(object):
  """Produces objects that represent customers."""
  def __init__(self, customer_id):
      self.customer_id = customer_id

  def display_cart(self):
      print "I'm a string that stands in for the contents of your shopping cart!"

class ReturningCustomer(Customer):
  """For customers of the repeat variety."""
  def display_order_history(self):
      print "I'm a string that stands in for your order history!"

monty_python = ReturningCustomer("ID: 12345")
monty_python.display_cart()
monty_python.display_order_history()
```

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 클래스 ReturningCustomer(Customer) 는 클래스 Customer 를 상속한다.    
• 클래스 ReturningCustomer 는 내부에 메서드 display_cart() 를 정의하지 않았다.    
• 그럼에도 불구하고, 객체(object) monty_python 은 .display_cart() 를 사용한다.
{: .notice--info}



**결과**     
``` 
I'm a string that stands in for the contents of your shopping cart!
I'm a string that stands in for your order history!
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 12. Inheritance Syntax    

In Python, inheritance works like this:    
```python
class DerivedClass(BaseClass):
    
# code goes here
```
where `DerivedClass` is the new class you're making and `BaseClass` is the class from which that new class inherits.



**설명:** [ Learn ]     
• Ch12. Inheritance Syntax 에서는 inheritance(상속) 문법을 학습한다.    
• 클래스(BaseClass)를 inhertance 하여 새로운 클래스(DerivedClass)를 만들려면,    
• DerivedClass의 ( ) 안에 상위 클래스 이름 (BaseClass) 을 넣으면 된다.     
• e.g. Class DerivedClass(BaseClass):
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* On lines 1-4, we've created a class named `Shape`.

* Create your own class, `Triangle`, that inherits from `Shape`, like this:    

```python
class Triangle(Shape):
# code goes here
```    

* Inside the `Triangle` class, write an `__init__()` function that takes four arguments: `self`, `side1`, `side2`, and `side3`.    

<p style="page-break-before: always;"></p>
<br>

* Inside the `__init__()` function, set `self.side1 = side1`, `self.side2 = side2`, and `self.side3 = side3`.    

* Click "Stuck? Get a hint!" for an example. 


**설명:** [ Instruction ]    
• 상위 클래스 Shape 를 inheritance 하는 새로운 클래스 Triangle 를 작성한다.        
• 클래스 Triangle 내부에는 다음과 같은 메서드가 있다.    
• e.g.  `def __init__(self, side1, dise2, side3):`    
• 메서드 `__init__()` 내부에는 다음을 작성한다.     
• e.g. self.side1 = side1    
• e.g. self.side2 = side2    
• e.g. self.side3 = side3
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)         
* Your code should look something like this:     


```python
class Triangle(Shape):
    def __init__(self, side1, side2, side3):
      self.side1 = side1
      self.side2 = side2
      self.side3 = side3
```    


**설명:** [ Hint ]     
• 클래스 Shape 를 inheritance 한 새로운 클래스 Triangle 정의하는 법을 참조한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python
class Shape(object):
    """Makes shapes!"""
    def __init__(self, number_of_sides):
      self.number_of_sides = number_of_sides

# Add your Triangle class below!
class Triangle(Shape):
    def __init__(self, side1, side2, side3):
      self.side1 = side1
      self.side2 = side2
      self.side3 = side3
```

**설명:** [ Solution ]     
• 클래스 Triangle(Shape) 는 클래스 Shape 를 inheritance 한다.    
• 메서드 `__init__()` 는 1 개 self 와 3 개의 매개변수(arguments)를 가진다.    
• 본문 내부에서는 self.side1 = side1 처럼 입력받은 arguments 를 매칭 시킨다.
{: .notice--info}



**결과**     
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 13. Override!    

Sometimes you'll want one class that inherits from another to not only take on the methods and attributes of its parent, but to **override** one or more of them.    
```python
class Employee(object):
    def __init__(self, name):
      self.name = name
    def greet(self, other):
      print "Hello, %s" % other.name

class CEO(Employee):
    def greet(self, other):
      print "Get back to work, %s!" % other.name

ceo = CEO("Emily")
emp = Employee("Steve")
emp.greet(ceo)
# Hello, Emily
ceo.greet(emp)
# Get back to work, Steve!
```    
Rather than have a separate greet_underling method for our CEO, we override (or re-create) the `greet` method on top of the base `Employee.greet` method. This way, we don't need to know what type of `Employee` we have before we `greet` another `Employee`.



**설명:** [ Learn ]     
• Ch13. Override! 에서는 오버라이딩을 학습한다.    
• Override(덮어쓰기) 에 대해서 알아보자.    
• Inheritance 는 상위 클래스의 속성과 메서드를 이용한다.    
• 속성과 메서드 를 포함한 전체를 가져오고 싶을때는 override 를 한다.    
• 오버라이딩은 클래스의 메서드를 객체의 사유에 따라 덮어쓰기를 할 수 있다.    
• ceo.greet()를 호출하면 *Get back to work, Emily* 가 출력될 것이라고 예상할 것이다.    
• ceo.greet(emp) 호출하면, *Get back to work, Steve* 가 호출된다.    
• 이유는 object(객체) emp 를 객체 ceo 가 override 하였기 때문이다.  
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a new class, `PartTimeEmployee`, that inherits from `Employee`.

* Give your derived class a `calculate_wage` method that overrides Employee's. It should take `self` and `hours` as arguments.

* Because `PartTimeEmployee.calculate_wage` overrides `Employee.calculate_wage`, it still needs to set `self.hours = hours`.

* It should return the part-time employee's number of `hours` worked multiplied by 12.00 (that is, they get $12.00 per hour instead of $20.00).




**설명:** [ Instruction ]    
• 클래스 Employee 를 inheritance 하는 PartTimeEmployee 를 작성하라.    
• 클래스 Employee 의 메서드 calculate_wage() 를 클래스 PartTimeEmployee 에서 override 하시오.    
• Override 한 calculate_wage(self, hours) 를 가진다.    
• Employee.calcuate_wage 의 override 한 것은 PartTimeEmployee.calculate_wage 이다.    
• 클래스 PartTimeEmployee 의 메서드 calculate_wage() 메서드는 다음을 가진다.    
• e.g. self.hours = hours    
• 클래스 PartTimeEmployee 의 메서드 calculate_wage(self, hours) 의 return 값은 ( hours x 12.00 ) 이다.    
• 참고로, 상위 클래스 PartTimeEmployee 의 메서드 calculate_wage() 의 return 값은 ( hours x 20.00 ) 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* In the example code above, we created an overriding `CEO.greet` method.     
* It had the same arguments as `Employee.greet`.     
* You'll want to add a `calculate_wage()` method to your `PartTimeEmployee` class, and it should also take `self` and `hours` as arguments.     
* Instead of returning `hours * 20.00`, though, it should return `hours * 12.00`.

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• 클래스 PartTimeEmployee 는 메서드 `__init__()` 는 정의하지 않는다.    
• 클래스 PartTimeEmployee 의 메서드 calculate_wage(self, hours) 를 가진다.    
• 클래스 PartTimeEmployee 의 메서드 calculate_wage()는 (hours x 12.00) 을 반환한다. 
{: .notice--info}

<br>
<hr/>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Employee(object):
    """Models real-life employees!"""
    def __init__(self, employee_name):
      self.employee_name = employee_name

    def calculate_wage(self, hours):
      self.hours = hours
      return hours * 20.00

# Add your code below!
class PartTimeEmployee(Employee):
    def calculate_wage(self, hours):
      self.hours = hours
      return hours * 12.00
```

**설명:** [ Solution ]     
• Override 한 PartTimeEmployee는 메서드 `__init__()`를 정의하지 않는다.    
• 내부 calculate_wage() 는 return 값을 ( hours * 12.00 ) 를 반환한다.
{: .notice--info}


**결과**     
``` 
#skip
```   
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 14. This Looks Like a Job For...    

On the flip side, sometimes you'll be working with a derived class (or subclass) and realize that you've overwritten a method or attribute defined in that class' base class (also called a parent or superclass) that you actually need. Have no fear! You can directly access the attributes or methods of a superclass with Python's built-in `super` call.

The syntax looks like this:    
```python
class Derived(Base):
    def m(self):
      return super(Derived, self).m()
```        
Where `m()` is a method from the base class.



**설명:** [ Learn ]     
• Ch14. This Looks Like a Job For... 에서는 오버라이딩, Super 를 학습한다.      
• 상위 클래스에 속해 있는 메서드를 수정 할려면, 함수 super() 를 이용한다.   
• 사용법은 super(Derived, self).m() 이라고 사용한다.    
• .m() 은 상위 클래스의 메서드를 가리킨다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* First, inside your `PartTimeEmployee` class:

* Add a new method called `full_time_wage` with the arguments `self` and `hours`.
* That method should return the result of a **super** call to the `calculate_wage` method of PartTimeEmployee's parent class.   

<p style="page-break-before: always;"></p>
<br>

* Use the example above for help.    

* Then, after your class:

* Create an instance of the `PartTimeEmployee` class called `milton`.    
* Don't forget to give it a **name**.    
* Finally, print out the result of calling his `full_time_wage` method.    
* You should see his wage printed out at **$20.00 per hour**! (That is, for 10 hours, the result should be 200.00.)



**설명:** [ Instruction ]    
• 클래스 PartTimeEmployee 의 메서드 full_time_wage(self, hours) 를 추가하라.    
• 메서드 full_time_wage() 는 super 를 이용하여 return 값을 반환한다.    
• return 값은 super 를 이용한다.     
• super 는 상위 클래스 Employee 의 calculate_wage() 의 결과값을 호출하여 사용한다.    
• 객체(objec) 를 다음과 같이 생성한다.    
• e.g. milton = PartTimeEmployee("peter")    
• 매개변수 parameter 에 이름을 넣는것을 잊지 말라.    
• 다음과 같이 호출 후, 출력하라.    
• e.g. print milton.full_time_wage(10)     
• 결과값은 '시간 x $20.00', 즉 200.00 이 출력 될 것이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You super call should look something like this:    

```python
def full_time_wage(self, hours):
    return super(PartTimeEmployee, self).method(args)
```       

* Where method is the method you want (`calculate_wage`) and args are the arguments that method takes.


**설명:** [ Hint ]     
• super 를 사용하는 방법을 참조하자.    
• .method(args) -> calculate_wage(name) 이라고 변경하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Employee(object):
    """Models real-life employees!"""
    def __init__(self, employee_name):
      self.employee_name = employee_name

    def calculate_wage(self, hours):
      self.hours = hours
      return hours * 20.00

# Add your code below!
class PartTimeEmployee(Employee):
    def calculate_wage(self, hours):
      self.hours = hours
      return hours * 12.00

    def full_time_wage(self, hours):
      return super(PartTimeEmployee, self).calculate_wage(hours)

milton = PartTimeEmployee('Milton')
print milton.full_time_wage(10)
```

**설명:** [ Solution ]     
• 메서드 full_time_wage() 를 다음과 같이 정의한다.    
• e.g. def full_time_wage(self, hours):      
• 결과값을 반환을 다음과 같이 한다.    
• e.g. return super(PartTimeEmployee, self).calculate_wage(hours)    
• 이 메서드는 상위클래스의 calculate_wage(hours) 를 호출한다.    
• 클래스 PartTimeEmployee('Milton') 의 instance 인 객체 milton 을 만든다.    
• e.g. milton.full_time_wage(10)    
• milton.full_time_wage(10) 호출후 출력한다.
{: .notice--info}


**결과**     
``` 
200.0
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 15. Class Basics    

First things first: let's create a class to work with.



**설명:** [ Learn ]    
• Ch15. Class Basics 에서는 실전 연습을 학습한다.         
• 실전 클래스를 만들어 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a class, `Triangle`.    
* Its `__init__()` method should take `self`, `angle1`, `angle2`, and `angle3` as arguments.     
* Make sure to set these appropriately in the body of the `__init__()` method (see the Hint for more).


**설명:** [ Instruction ]    
• 클래스 Triangle 를 작성하라.    
• 클래스 Triangle 는 다음의 메서드를 가진다.    
• e.g. `def __init__(self, angle1, angle2, angle3):`    
• 메서드 `init__()` 의 내부에는 다음고 같이 매칭하도록 추가한다.    
• e.g. self.angle1 = angle1    
• e.g. self.angle2 = angle2    
• e.g. self.angle3 = angle3
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
<p style="page-break-before: always;"></p>
<br>

* Make sure your Triangle inherits from object.     
* Remember, class syntax looks like this:    

```python
class ClassName(object):
    def __init__(args):
      # Set self.args = args
```

**설명:** [ Hint ]     
• 클래스 Triangle 는 클래스 object 를 상속한다.    
• 클래스를 만드는 문법을 참고한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Triangle(object):
    def __init__(self, angle1, angle2, angle3):
      self.angle1 = angle1
      self.angle2 = angle2
      self.angle3 = angle3
```

**설명:** [ Solution ]     
• 클래스 Triangle 은 (object)를 inhertance 한다.    
• 메서드 `__init__(self, angle1, angle2, angle3)` 를 parameter를 가진다.    
• `__init__()` 의 내부를 초기화 한다.    
• e.g. self.angle1 = angle1    
• e.g. self.angle2 = angle2    
• e.g. self.angle3 = angle3
{: .notice--info}


**결과**     
``` 
#skip
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 16. Class It Up    

Great! Now let's **add** a **member variable** and a **method** to our class.


<br>
**설명:** [ Learn ]    
• Ch16. Class It Up 에서는 클래스 변수와 메서드를 학습한다.     
• member variable 와 method 를 추가해 보자.
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside the `Triangle` class:    

* Create a variable named `number_of_sides` and set it equal to 3.    

* Create a method named `check_angles`.    
* The sum of a triangle's three angles should **return True** if the sum of `self.angle1`, `self.angle2`, and `self.angle3` is equal 180, and False otherwise.



**설명:** [ Instruction ]    
• 클래스 Triangle 안에 다음 내용을 추가 하시오.   
• number_of_sides = 3    
• def check_angles(self):   
• 메서드 check_angles() 는 True or False 를 반환한다.        
• True : self.angle1 + self.angle2 + self.angle3 = 합이 180    
• False : True 가 아닌 경우.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* The check_angles method should look something like this:      

```python
def check_angles(self):
    if (self.angle1 + self.angle2 + self.angle3 == 180):
      return True
    else:
      return False
```

**설명:** [ Hint ]     
• 클래스 변수(member variables)를 추가하라.    
• 메서드 check_angles(self) 는 매개변수(parameter) self 만 가진다.    
• 메서드 작성 방법을 참조하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Triangle(object):
    number_of_sides = 3
    def __init__(self, angle1, angle2, angle3):
      self.angle1 = angle1
      self.angle2 = angle2
      self.angle3 = angle3
      
    def check_angles(self):
      if (self.angle1 + self.angle2 + self.angle3) == 180:
        return True
      else:
        return False
```

**설명:** [ Solution ]     
• 클래스(member) 변수 number_of_sides = 3 를 추가한다.    
• 메서드 check_angles(): 추가한다. ( e.g. def check_angles(self): )   
• 클래스에서 입력받은 parameter 값을 합하여 180 이면 True 를 반환한다.    
• 그 외는 False 를 반환한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

**결과**     
``` 
#skip
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 17. Instantiate an Object    

Let's go ahead and create an **instance** of our `Triangle` class.


<br> 

**설명:** [ Learn ]     
• Ch17. Instantiate an Object 에서는 Instance 학습한다.    
• 클래스 Triangle 의 instance를 만들어 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable named `my_triangle` and set it equal to a new instance of your `Triangle` class.     
* Pass it three angles that sum to 180 (e.g. 90, 30, 60).

* Print out my_triangle.number_of_sides

* Print out my_triangle.check_angles()




**설명:** [ Instruction ]    
• 클래스 Triangle 의 instance 인 객체(object) my_triangle 를 작성하라.    
• parameter 값으로 3 개 합이 180 이 되게 넣는다.    
• e.g. a=90, b=30, c=60       
• Instance 한 객체 my_triangle 의 변수 number_of_sides 를 호출후 출력한다.      
• e.g. print my_triangle.number_of_sides    
• Instance 한 객체 my_triangle 의 메서드 check_angles() 를 호출후 출력한다.    
• e.g. print my_triangle.check_angles()
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, we can instantiate an `object` like so:     

```python
instance = Class(args)

```
* Where args are the arguments `__init__()` takes, not including self.


**설명:** [ Hint ]     
• Iinstance 한 객체(object)를 만드는 법을 참조하라.        
• 매개변수(arguments)에는 self 가 들어가지 않는다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Triangle(object):
    number_of_sides = 3
    def __init__(self, angle1, angle2, angle3):
      self.angle1 = angle1
      self.angle2 = angle2
      self.angle3 = angle3
      
    def check_angles(self):
      if (self.angle1 + self.angle2 + self.angle3) == 180:
        return True
      else:
        return False
  
my_triangle = Triangle(30, 60, 90)

print my_triangle.number_of_sides
print my_triangle.check_angles()

```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Solution ]     
• 객체(object) my_triangle 를 작성한다.    
• 이 객체는 클래스 Triangle(30, 60, 90)을 instance 한다.    
• 객체(object) my_triangle 의 클래스 변수 number_of_sides 를 호출한다.    
• 그리고 그 결과값을 출력한다.    
• 객체(object) my_triangle 의 메서드 check_angles() 를 호출한다.    
• 그리고 그 결과값을 출력한다.
{: .notice--info}

**결과**     
``` 
3
True
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 

### 18. Inheritance    

Finally, let's create an `Equilateral` class that **inherits** from our `Triangle` class. (An equilateral triangle is a triangle whose angles are all 60˚, which also means that its three sides are equal in length.)



**설명:** [ Learn ]    
• Ch18. Inheritance 에서는 상속(inheritance)을 학습한다.      
• 클래스 Triangle 를 inheritance 한 클래스 Equilateral 를 만들어 보자.    
• Equilateral 은 3 각 모두가 60˚ 인 삼각형이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a class named `Equilateral` that **inherits** from `Triangle`.

* Inside `Equilateral`, create a member variable named `angle` and set it equal to 60.

* Create an `__init__()` function with only the parameter `self`, and set `self.angle1`, `self.angle2`, and `self.angle3` equal to `self.angle` (since an equilateral triangle's angles will always be 60˚).




**설명:** [ Instruction ]    
• 클래스 Triangle 를 inheritance 한 클래스 Equilateral 를 작성하라.        
• 클래스 Equilateral 내부에는 클래스(member) 변수인 angle = 60 을 작성하라.      
• 내부에 메서드 `__init__(self)` 를 작성하라.      
• 내부 메서드의 변수 3 개를 다음과 같이 초기화 하라.    
• e.g. self.angle1 = angle     
• e.g. self.angle2 = angle     
• e.g. self.angle3 = angle
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, **inheritance** looks like this:      

```python
class DerivedClass(BaseClass):
# Your code here
```      

* where `DerivedClass` is the new class you're making, and `BaseClass` is the class it **inherits** from.


**설명:** [ Hint ]     
• Inheritance 는 상위 클래스의 속성과 메서드를 상속 받는다.       
• Inheritance 를 했기에, partamerter 도 inheritance 된다.      
• 예제를 참고하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Triangle(object):
    number_of_sides = 3
    def __init__(self, angle1, angle2, angle3):
      self.angle1 = angle1
      self.angle2 = angle2
      self.angle3 = angle3
      
    def check_angles(self):
      if (self.angle1 + self.angle2 + self.angle3) == 180:
        return True
      else:
        return False
```
<p style="page-break-before: always;"></p>
<br>

```python
class Equilateral(Triangle):
    angle = 60
    def __init__(self):
      self.angle1 = self.angle
      self.angle2 = self.angle
      self.angle3 = self.angle
```    

**설명:** [ Solution ]     
• 클래스 Equilateral 은 클래스 Triangle 를 inheritance 하여 정의한다.    
• 클래스(member) 변수에 60 을 할당한다.    
• 메서드 `__init__(self)` 를 정의한다. 이때, 매개변수(arguments)가 없다.    
• 이유는 inheritance 했기 때문이다.     
• 하지만, 초기화는 다음과 같다.     
• e.g. self.angle1 = self.angle
{: .notice--info}


**결과**     
``` 
#skip
```   

