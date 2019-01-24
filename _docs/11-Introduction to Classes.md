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

* Remove the pass statement in your class definition, then go ahead and define an __init__() function for your Animal class.     
* Pass it the argument self for now; we'll explain how this works in greater detail in the next section.     
* Finally, put the pass into the body of the __init__() definition, since it will expect an indented block.

 


**설명:** [ Instruction ]    
• 키워드 pass 를 제거하고, 그자리에 `__init__()`를 정의하라.    
• `__init__()`는 기본적으로 `self` argument를 가진다.    
• `__init_()` 내부에 키워드 pass 를 넣어라.    
•  단, 들여쓰기(indented block)를 주의하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Your __init__() function should look something like this:
```python
def __init__(self):
  pass
```

**설명:** [ Hint ]     
• __init__() 사용법을 참조하라.
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
• 내부 메서드 __init__(self)를 선언한다. 
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

So far, __init__() only takes one parameter: self. This is a Python convention; there's nothing magic about the word self. However, it's overwhelmingly common to use self as the first parameter in __init__(), so you should do this so that other people will understand your code.

The part that is magic is the fact that self is the first parameter passed to __init__(). Python will use the first parameter that __init__() receives to refer to the object being created; this is why it's often called self, since this parameter gives the object being created its identity.



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
### 5. 



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
### 6. 



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
### 7. 



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
### 8. 



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
### 9. 



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
