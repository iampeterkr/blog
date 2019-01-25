---
# layout : rchive
title: "Introduction to Classes"
permalink: /introduction-classes-/
excerpt: "We learn about Classes Syntax."
last_modified_at: 2019-01-24T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
<hr style="border: solid 1px #dddddd ;">    

LESSON    

Classes are a crucial part of object-oriented programming (OOP). In this lesson, we'll explain what classes are, why they're important, and how to use them effectively.

**설명:** [ 학습방향 ]     
클래스는 객체지향의 끝판황이라 할수 있다. 이 장에서는, 우리는 클래스가 무엇이며, 왜 중요하며, 어떻게 효과적으로 사용하는지를 배우겠다.
{: .notice--info}     
     
 <hr style="border: solid 1px #dddddd ;">

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


**설명:** [ Learn ]     
• Python은 객체지향 프로그램이다. 객체지향이란, 객체(objects)라고 불리는 것을 조작할수 있는 프로그램이다.    
• 우리는 함수(function)라는것을 배웠다. 이것도 하나의 객체(objects)이다.     
• 함수는 우리가 외부에서 arguments로 입력값을 조절하며, 결과값을 구할 수 있었다.    
• 함수의 또다른 이름은 메서드(methods)라고 한다.    
• 이런 메서드들을 모아 놓은 것을 클래스라 한다. 
• 클래스를 함수=메서드=객체의 개념적 틀이라고 일단 생각하자.    
• 여기서는 여기까지 개념을 잡고, 더 자세한 내용은 다음 장에서 설명하겠다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor to the right.     
* We've defined our own **class**, Fruit, and created a lemon **instance**.    
* When you're ready, click Run to get started creating classes and objects of your own. 


**설명:** [ Instruction ]    
* edit 창의 소스를 분석해 보자.    
* Fruit 클래스, lemon instance가 정의 되어 있다.    
* Run을 클릭하면, 자신만의 클래스와 객체(objects) 만들어 진다. 
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
• 클래스 Fruit(object) 가 정의되어 있다. 이것은 object를 상속 받고 있다.    
• object 상속의 개념은 추후에 설명할 것이다.    
• 클래스 Fruit(object)에는 3개의 메소드가 정의되어 있다.    
• 클래스 밖에는 lemon 이라는 객체가 만들어 진다.     
• 이 lemon 객체는 Fruit 클래스의 instance 를 가진다.    
• 객체 lemon을 통하여 Fruit 클래스의 description() 메서드를 호출한다.    
• 객체 lemon을 통하여 Fruit 클래스의 is_edible() 메서드를 호출한다.  
{: .notice--info}


**결과**     
``` 
I'm a yellow lemon and I taste sour.
Yep! I'm edible.
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 2.  Class Syntax    

A basic class consists only of the `class` keyword, the name of the class, and the class from which the new class **inherits** in parentheses. (We'll get to inheritance soon.)     
For now, our classes will **inherit** from the object class, like so:
```python
class NewClass(object):
  # Class magic here
```
This gives them the powers and abilities of a Python object.     
By convention, user-defined Python class names start with a capital letter.



**설명:** [ Learn ]     
• 클래스의 문법을 알아보자.     
• `class 클래스 이름 (objects)`    
• `class` : 이 정의된 것이 클래스임을 알려줌.    
• `클래스 이름` : 메서드들을 대표할수 있는 이름을 적어줌.    
• `(objects)`: objects 의 기능을 상속(inherits) 받는다.    
• `(objects)`라고 선언하면 Pythond object의 기능을 활용할수 있게 해준다.    
• Python은 클래스 이름을 쓸때, capital letter 방식으로 정의한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a class called `Animal` in the editor.     
* For now, in the body of your class, use the `pass` keyword. (pass doesn't do anything, but it's useful as a placeholder in areas of your code where Python expects an expression.) 


**설명:** [ Instruction ]    
• 클래스 Animal을 만들어라.    
• 클래스 Animal 내부에 pass 키워드를 사용하라.    
• pass 는 추후에 설명하겠다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Use the example in the instructions as a guide!


**설명:** [ Hint ]     
• 상단의 클래스 함수 정의 한것을 참조하라. 
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
• Animal 내부에 pass 키워드를 넣었다.
{: .notice--info}


**결과**     
``` 
skip
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 3. Classier Classes    

We'd like our classes to do more than... well, nothing, so we'll have to replace our pass with something else.

You may have noticed in our example back in the first exercise that we started our class definition off with an odd-looking function: __init__(). This function is required for classes, and it's used to initialize the objects it creates. __init__() always takes at least one argument, self, that refers to the object being created. You can think of __init__() as the function that "boots up" each object the class creates.

 



**설명:** [ Learn ]     
• 클래스 내부의 키워드 pass 자리에 어떤 기능들을 구현하여야 한다.     
• 클래스 1장에서 클래스를 소개하면서 보여준 소스에서, `__init__()`메서드를 보았다.    
• `__init__()`는 클래스에서 반드시 필요한 메서드이다.    
• `__init__()`는 클래스 객체가 생성될때, 초기화 하는데 사용되어진다.    
• `__init__()`는 최소한 1개의 argument `self` 를 가진다.    
• `__init__()`는 객체가 생성될때마다 실행되는 함수이자 메서드이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Remove the pass statement in your class definition, then go ahead and define an `__init__()` function for your Animal class.     
* Pass it the argument self for now; we'll explain how this works in greater detail in the next section.     
* Finally, put the pass into the body of the `__init__()` definition, since it will expect an indented block.

 


**설명:** [ Instruction ]    
• 키워드 pass 를 제거하고, 그자리에 `__init__()`를 정의하라.    
• `__init__()`는 기본적으로 `self` argument를 가진다.    
• `__init_()` 내부에 키워드 pass 를 넣어라.    
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
• 클래스 Animal(object)를 정의한다.    
• 내부 메서드 `__init__(self)`를 선언한다. 
• 그안에 pass 키워드를 입력한다. 
{: .notice--info}



**결과** 
``` 
skip
```

<br>
<br>    
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
• `__inti__()`는 `self`를 매개변수를 가진다. 이것은 Python 약속이다.    
• `self`가 특별한 것은 없지만, 무조건 `__inti__()`첫번째 매개변수로 사용된다.    
• 클래스가 호출되면, 자동으로 `__init__(slef)`가 호출된다.     
• 호출될때, 자기 자신을 호출하기에, `self`라고 부른다.    
• `self`가 호출되는것은 이 객체의 정체성(누구 것인지)를 알게 해준다.     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Let's do two things in the editor:

* Pass `__init__()` a second parameter, `name`.    

* In the body of `__init__()`, let the function know that `name` refers to the created object's `name` by typing `self.name = name.` (This will become crystal clear in the next section.)
 


**설명:** [ Instruction ]    
• `__init__(self)`의 두번째 매개변수(parameter)에 name을 넣자.    
• `__init__(self, name)`의 내부에 `self.name = name`라고 하자.
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
• `__init__(self, namee)`에 두번째 매개변수에 `name`을 정의하자.    
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
• `def __init__(self, name):`를 정의한다.    
• `self.name = name`이라고 정의한다.     
• 이 뜻은 매개변수 `name`의 값을 `self.name`에 저장한다는 뜻이다.
{: .notice--info}



**결과**     
``` 
skip
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 5. Instantiating Your First Object    

Perfect! Now we're ready to start creating objects.

We can access attributes of our objects using dot notation. Here's how it works:
```python
class Square(object):
  def __init__(self):
    self.sides = 4

my_shape = Square()
print my_shape.sides 
# my_shape. 찍는순간 __init__(self)가 호출된다.
```
* First we create a class named Square with an attribute sides.
* Outside the class definition, we create a new instance of Square named my_shape and access that attribute using my_shape.sides.


**설명:** [ Learn ]      
• 클래스의 기본은 만들어 졌다. 우리는 객체를 만들수 있다.     
• `.`을 사용하여 우리는 객체의 속성에 접근할수가 있다.    
• `my_shape = Square()`는 클래스 Square()의 속성을 그대로 사용할수 있는    
•  Object(객체) `my_shape`가 만들어 진다.    
• `my_shape`객체는 `Square()`의 내부 속성을 사용할려면,     
• `my_shape.` 이라고 `.`을 찍는 순간 클래스의 `__init__(self)`가 호출된다.    
• `my_shape.sides`는 `__init__(self)`의 `self.sides`에 접근할수가 있다.    
• `self.sides = 4` 이기에,    
• `print my_shape.sides`는 4가 출력된다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Outside the `Animal` class definition, create a variable named `zebra` and set it equal to `Animal("Jeffrey")`.

* Then print out zebra's name. 


**설명:** [ Instruction ]    
• 클래스 `Animal` 바깥에, 변수 `zebra`를 만들어라.    
• `zebra = Animal("Jeffrey")` 선언하라.(객체 생성)      
• zebra의 이름을 출력하라.

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
• Animal 클래스를 사용하는 객체(object) zebra를 생성한다.    
• zebra.name을 호출하면, 클래스 Animal의 name에 있는 내용이 출력된다.
{: .notice--info}

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
• `zebra = Animal("Jeffrey")`    
• 클래스 Animal을 instance 하는 객체 `zebra`를 생성한다.   
• 클래스 Animal()의 파라메터에 값 "Jeffrey"를 넣는다.    
• 변수 `name`에는 "Jeffrey"가 넘겨진다.
• 객체 `zebra`는 클래스 Aniaml의 속성을 그대로 가지고 있다.    
• `zebra.`하는 순간 클래스 Animal()의 `__init__(self)`가 호출된다.    
• `zebra.name`은 클래스 Animal의 name이 출력된다.
{: .notice--info}



**결과**     
``` 
Jeffrey
```

<br>
<br>    
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
• 객체를 생성할때, `__init__(self)`가 호출된다.     
• self 외에도 name, age 매개 변수를 추가할 수 있다.    
• `__init__()` 호출되면 내부에는 self.name, self.age 가 만들어진다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the examples in the editor.     
* See how `__init__()` "boots up" each object to expect a `name` and an `age`, then uses `self.name` and `self.age` to assign those names and ages to each object?     
* Add a third attribute, `is_hungry` to `__init__()`, and click Run to see the results.


**설명:** [ Instruction ]    
• `__init__()`에 `is_hungry`를 세번재 매개변수로 추가하여라.    
• 실행시켜 보아라. 그리고 결과를 지켜보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your code should look something like this:
```python
def __init__(self, name, age, is_hungry)
  self.name = name
  self.age = age
  self.is_hungry = is_hungry
```


**설명:** [ Hint ]     
• `is_hungry`를 세번째 매개변수로 추가한다.     
• `self.is_hungry = is_hungry`로 정의한다. 
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
• `def __init__(self, name, age, is_hungry):`    
• 세번째 매개변수 `is_hungry`를 추가하였다.    
• `self.is_hungry = is_hungry`    
• 세번째 매개변수를 매칭 시켜 준다.   
{: .notice--info}



**결과**     
``` 
Jeffrey 2 True
Bruce 1 False
Chad 7 True
```

<br>
<br>    
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
• 클래스에서 중요한게 변수의 주기(scope)이다.      
• 우리는 변수는 한번 생성되면 계속 접속 할수 있다고 생각한다.      
• 클래스 변수에는 3종류가 있다.    
  `-` 전역변수(global variables):어디서든 접근 가능    
  `-` 변수(member variables) : 클래스 멤버만 접근 가능    
  `-` instance variables:클래스의 객체만 접근 가능 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Check out the code in the editor.     
* Note that each individual animal gets its own `name` and `age` (since they're all initialized individually), but they all have access to the member variable `is_alive`, since they're all members of the `Animal` class.     
* Click Run to see the output! 


**설명:** [ Instruction ]    
• `name`, `age`는 instance 변수 이다.        
• `is_alive`는 클래스 변수 이다.     
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

**설명:** [ Solution ]     
• `is_alive`는 클래스 변수이다.    
• `name`, `age`는 instance 변수이다. 
{: .notice--info}



**결과**     
```
Jeffrey 2 True
Bruce 1 True
Chad 7 True
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 8. A Methodical Approach    

When a class has its own functions, those functions are called **methods**. You've already seen one such method: `__init__()`. But you can also define your own methods!



**설명:** [ Learn ]     
• 클래스가 가지고 있는 함수를 메서드(method) 라고 부른다.    
• `__init__()`도 클래스의 메서드 이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Add a method, `description`, to your `Animal` class.     
* Using two separate print statements, it should print out the `name` and `age` of the animal it's called on.     
* Then, create an instance of Animal, `hippo` (with whatever name and age you like), and call its `description` method. 


**설명:** [ Instruction ]    
• Animal 클래스에 메서드 description()를 추가하여라.     
• description()는 동물의 이름(name)과 나이(age)를 출력(print)한다.    
• Animal 클래스의 instance를 가진 hippo를 만드시오.(ex.`hippo = Animal()`)    
• 그 객체(object) hippo의 메서드(method)인 description()를 호출하라.  
{: .notice--info}


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
• 메서드 description(self)은 self parameter가 있어야 한다.
• 메서드 description()가 호출되면, name과 age가 출력된다.    
• hippo.description() 으로 호출 한다. 
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

**설명:** [ Solution ]     
• 클래스 Animal 내부에 description(self) 메서드를 만들었다.    
• 메서드 description(self)는 name과 age를 출력한다.    
• 클래스 Animal("Anderson", 36)을 instance 하는 object(객체) hippo를 생성한다.    
• object(객체)를 이요하여, 메서드 description()을 호출한다.  
{: .notice--info}



**결과**     
``` 
Anderson
36
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 9. They're Multiplying!    

A class can have any number of member variables. These are variables that are available to all members of a class.

hippo = Animal("Jake", 12)
cat = Animal("Boots", 3)
print hippo.is_alive
hippo.is_alive = False
print hippo.is_alive
print cat.is_alive
In the example above, we create two instances of an Animal.
Then we print out True, the default value stored in hippo's is_alive member variable.
Next, we set that to False and print it out to make sure.
Finally, we print out True, the value stored in cat's is_alive member variable. We only changed the variable in hippo, not in cat.
Let's add another member variable to Animal.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 10. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 11. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 12. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}



**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 13.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 14. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

**결과**     
``` 
```   

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 15.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 16. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 17.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 18.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">INTRODUCTION TO CLASSES</font> 
### 19.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

① 


**설명:** [ Instruction ]    
① 

{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** [ Hint ]     

{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** [ Solution ]     

{: .notice--info}


**결과**     
``` 
```   


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
