---
# layout : rchive
title: "Classes"
permalink: /classes/
excerpt: "We learn about Classes Syntax."
# last_modified_at: 2019-01-26T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
     
     

<hr style="border: solid 1px #dddddd ;">    
LESSON    

Make your own Car and learn how to driveCar()!    


**설명:** [ 학습방향 ]     
이 장에서는 자동차를 가지고 작은 프로젝트를 단계별 진행하면서 클래스에 대하여 좀 더 깊이 있게 이해하고 연습해 보자. 
{: .notice--info}     
     
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 1.  Class basics    

Classes can be very useful for storing complicated objects with their own methods and variables. Defining a class is much like defining a function, but we use the class keyword instead. We also use the word object in parentheses because we want our classes to inherit the object class. This means that our class has all the properties of an object, which is the simplest, most basic class. Later we'll see that classes can inherit other, more complicated classes. An empty class would look like this:
```python
class ClassName(object):
  # class statements go here
```



**설명:** [ Learn ]     
• Ch1.  Class basics 에서는 클래스에 기본 정의를 학습한다.      
• 클래스는 여러가지 유용한 것들이 많다.    
• 메서드와 변수들이 섞여 있는 객체를 만드는데 유용하다.    
• 클래스간 Inherits(상속)를 할 수 있다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a new class named "Car".     
* For now, since we have to put something inside the class, use the `pass` keyword. 


**설명:** [ Instruction ]    
• 클래스 Car 를 만들어라.    
• 클래스 내부에 pass 키워드를 넣어라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Class has an object as argument

**설명:** [ Hint ]    
• class Car (object):
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  pass
```

**설명:** [ Solution ]     
• 클래스 Car 를 만들었다.    
• 클래스 Car 는 object 를 가진다.
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
<font size="3"  face="돋움">CLASSES</font>     

### 2. Create an instance of a class    

We can use classes to create new **objects**, which we say are **instances** of those classes.

Creating a new instance of a class is as easy as saying:
```python
newObject = ClassName()
``` 


**설명:** [ Learn ]      
• Ch2. Create an instance of a class 에서는 클래스 인스탄스를 학습한다.     
• 클래스를 사용하는 방법은 다음과 같다.    
• 클래스 ClassName() 를 instance 하는 object newObject 를 만든다.    
• newObject = ClassName()
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your `Car` class, create a new object named `my_car` that is an instance of `Car`. 


**설명:** [ Instruction ]    
• 클래스 Car 를 instance 하는 object my_car 를 작성하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Reference the description above, how to make new instance

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• 상단의 instace를 만드는 방법을 참조하시오.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  pass

my_car = Car()
```

**설명:** [ Solution ]     
• 클래스 Car()를 instance 하는 object my_car를 생성하였다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 3. Class member variables    

Classes can have **member variables** that store information about each class object. We call them **member variables** since they are information that belongs to the class object.

Creating **member variables** and assigning them initial values is as easy as creating any other variable:
```python
class ClassName(object):
  memberVariable = "initialValue"
``` 



**설명:** [ Learn ]       
• Ch3. Class member variables 에서는 클래스(member) 변수를 학습한다.    
• member 변수는 클래스 object 내부에 있는 변수이다.    
• member 변수를 만들고 초기화 한다.    
• e.g. memberVariable = "initialValue"
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside your `Car` class, replace the `pass` statement with a new member variable named `condition` and give it an initial value of the string "new". 


**설명:** [ Instruction ]    
• 클래스 Car 안에 있는 pass 를 삭제하라.    
• 그 자리에 member 변수 condition 을 작성하라.    
• member 변수 condition 을 초기화 하라.    
• e.g. condition = "new"
{: .notice--info}


<p style="page-break-before: always;"></p>
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
class Car(object):
  condition = "new"

my_car = Car()
```

**설명:** [ Solution ]     
• member 변수 condition 에 초기값 "new"를 저장한다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 4. Calling class member variables    

Each class object we create has its own set of **member variables**. Since we've created an object `my_car` that is an instance of the `Car` class, `my_car` should already have a member variable named `condition`. This attribute gets assigned a value as soon as `my_car` is created.





**설명:** [ Learn ]        
• Ch4. Calling class member variables 에서는 클래스 변수 호츨을 학습한다.    
• object my_car 를 만들면,     
• 클래스 Car 에서 선언된 member 변수 condition 이 자동으로 할당된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* At the end of your code, use a print statement to display the `condition` of `my_car`. 


**설명:** [ Instruction ]    
• object my_car 의 member 변수 condition 을 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Since the attribute condition belongs to the object `my_car`, you'll need to use **dot** notation to access the object's member variable:     

```python
my_car.condition.
```
<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]     
• 클래스(member) 변수를 불러올때는 Dot( . ) 을 사용한다.     
• e.g. my_car.condition
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  condition = "new"

my_car = Car()

print my_car.condition
```

**설명:** [ Solution ]     
• object my_car 의 member 변수 condition 을 호출하고 출력한다. 
{: .notice--info}



**결과**     
``` 
new
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 5. Initializing a class    

There is a special function named `__init__()` that gets called whenever we create a new instance of a class. It exists by **default**, even though we don't see it. However, we can define our own `__init__()` function inside the class, overwriting the default version. We might want to do this in order to provide more input variables, just like we would with any other function.

The first argument passed to `__init__()` must always be the keyword `self` - this is how the object keeps track of itself internally - but we can pass additional variables after that.

In order to assign a variable to the class (creating a member variable), we use **dot** notation. For instance, if we passed newVariable into our class, inside the `__init__()` function we would say:
```python
self.new_variable = new_variable
```



**설명:** [ Learn ]       
• Ch5. Initializing a class 에서는 클래스 초기화를 학습한다.    
• 객체를 만들기 위해서 클래스를 호출하면, 해당 클래스의 `__init__()` 이 호출된다.    
• 클래스 내에 있는 기본 `__init__()` 를 우리가 추가 정의 할수도 있다.    
• `__init__(self)` 첫번째, argument 는 무조건 self 이다.    
• 객체가 self 를 이용하여 자신을 추적한다.    
• 첫번째 arguments 인 self 외에도 a, b, c 와 같이 여러개의 변수를 전달할 수 있다.    
• e.g. `__init__(self, a, b, c)`     
•  클래스에 접근하기 위해선, Dot ( . ) 을 이용하여야 접근이 가능 하다.    
• `__init__()` 에 값이 전달되면 다음과 같이 메서드 내부에 값을 전달할수 있다.    
• e.g. self.new_variable = new_variable  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

<p style="page-break-before: always;"></p>
<br>

* Define the `__init__()` function of the `Car` class to take four inputs: `self`, `model`, `color`, and `mpg`. Assign the last three inputs to member variables of the same name by using the `self` keyword.

* Then, modify the object `my_car` to provide the following inputs at initialization:

```python
model = "DeLorean"
color = "silver"
mpg = 88
```

* You don't need to include the `self` keyword when you create an instance of a class, because `self` gets added to the beginning of your list of inputs automatically by the class definition.

 


**설명:** [ Instruction ]    
• 클래스 Car 안에 메서드 `__init__(self, model, color, mpg)`를 만들어라.    
• 메서드 `__init__()` 내부에 입력된 instance 변수를 self 를 이용하여 초기화 하여라.    
• 클래스 Car 를 instance 한 object my_car 를 아래 값들을 이용하여 수정하라.    
• 다음과 같이 수정후, 호출한다.    
• e.g. my_car = Car(model="DeLorean", color = "silver", mpg=88)    
• 참고로, object my_car를 생성할때, Car(self, a, b, c) self 를 넣지 않아도 된다.    
• 그 이유는 넣지 않아도, 자동으로 self 가 입력된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Creating an instance of a class with many initialization variables looks the same as calling a function with many inputs; put all the values in parentheses, separated by commas.

* In the body of `__init__()`, you'd set the model like this:    

```python
def __init__(self, model, color, mpg):
  self.model = model
```


**설명:** [ Hint ]     
• 클래스의 instance를 만들때, 아래와 같이 변수 값을 지정할 수 있다.    
• e.g. instance 변수 model 만 초기화 함.    
• e.g. self.model = model
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg

my_car = Car("DeLorean", "silver", 88)
```

**설명:** [ Solution ]     
• 함수 `__init__(self, model, color, mpg):` 의 변수 초기화는 다음과 같다.    
• e.g. self.model = model  
• my_car를 만들때, instance 변수 초기값("DeLorean", "silver", 88)을 넣는다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 6. Referring to member variables   

Calling class member variables works the same whether those values are created within the class (like our car's condition) or values are passed into the new object at initialization. We use dot notation to access the member variables of classes since those variables belong to the object.

For instance, if we had created a member variable named new_variable, a new instance of the class named new_object could access this variable by saying:
```python
new_object.new_variable
```



**설명:** [ Learn ]       
• Ch6. Referring to member variables 에서는 클래스 변수 참조하는 방법을 학습한다.    
• member 변수는 클래스가 만들어질때 값이 초기화 된다.    
• 또는, 객체가 생성될때 전달되기도 한다.    
• 클래스(member) 변수는 Dot ( . ) 을 사용하여 접근 할 수 있다.     
• 사용법은 다음과 같다.    
• e.g. new_object.new_variable
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Now that you've created `my_car` print its member variables:

* First print the `model` of `my_car`. Click "Stuck? Get a hint!" for an example.
* Then print out the `color` of `my_car`.
* Then print out the `mpg` of `my_car`.
 
<p style="page-break-before: always;"></p>
<br>


**설명:** [ Instruction ]    
• my_car 의 member 변수를 출력하라.    
• my_car 의 instance 변수 model 을 출력하라.    
• my_car 의 instance 변수 color 를 출력하라.    
• my_car 의 instance 변수 mpg 를 출력하라.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To print my_car's model, you'd type:    

```python
print my_car.model
```


**설명:** [ Hint ]     
• Object my_car 의 instance 변수 model 을 참조하는 방법이다.    
• my_car.model 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg

my_car = Car("DeLorean", "silver", 88)

# model = "DeLorean"
# color = "silver"
# mpg = 88
# my_car = Car(model, color, mpg)
```
<p style="page-break-before: always;"></p>
<br>

```python
print my_car.model
print my_car.color
print my_car.mpg
```

**설명:** [ Solution ]     
• 생성된 my_car 의 instance 변수 model, color, mpg 를 호출하여 출력한다.
{: .notice--info}



**결과**     
``` 
DeLorean
silver
88
```    
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 7. Creating class methods    

Besides member variables, classes can also have their own methods. For example:

```python
class Square(object):
  def __init__(self, side):
    self.side = side

  def perimeter(self):
    return self.side * 4
```
The `perimeter()` class method is identical to defining any other function, except that it is written inside of the Square class definition.

Just like when we defined `__init__()`, you need to provide `self` as the first argument of any class method.



**설명:** [ Learn ]       
• Ch7. Creating class methods 에서는 클래스안의 메서드를 만드는 방법을 학습한다.    
• 클래스 안에는 `__init__()` 외에도 다른 메서드를 만들수 있다.    
• 메서드 perimeter() 는 클래스 내의 다른 메서드에서 정의된 부분을 제외하고 정의하였다.    
• 메서드는 무조건 첫번째 인자는 self 이다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside the `Car` class, add a method named `display_car` to `Car` that will reference the Car's member variables to return the string,     
* "This is a [color] [model] with [mpg] MPG."     

<p style="page-break-before: always;"></p>
<br>

* You can use the `str()` function to turn your `mpg` into a string when creating the display string.   
* Replace the individual print statements with a single print command that displays the result of calling `my_car.display_car()`

  


**설명:** [ Instruction ]    
• 클래스 Car 내부에 메서드 display_car() 를 정의하라.    
• 메서드 display_car()는 color, model, mpg 를 반환한다.    
• mpg 는 문자열 str(mpg) 로 변경 후 반환한다.    
• my_car.display_car()를 호출하면, 각각의 color, model, mpg를 출력한다. 
{: .notice--info}

<br>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember, in order to access member variables of a class (even while inside of that class), we have to use the self keyword and dot notation to specify that we mean the member variable that belongs to the class.

```python
def display_car(self):
  print self.color

```  

**설명:** [ Hint ]     
• 클래스의 member 변수에 접근하기 위해선 Dot ( . ) 을 사용한다.     
• 메서드 display_car(self) 내부에서 변수를 사용할때는 다음과 같이 사용한다.    
• e.g. self.color
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>

```python    
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg
   
  def display_car(self):
    print "This is a %s %s with %s MPG." % (self.color, self.model, str(self.mpg))

my_car = Car("DeLorean", "silver", 88)

my_car.display_car()
```

**설명:** [ Solution ]     
• 메서드 display_car(self) 에서 color, model, mpg를 사용할때는 self 를 사용한다.
{: .notice--info}



**결과**     
``` 
This is a silver DeLorean with 88 MPG.
```      
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 8. Modifying member variables    

We can modify variables that belong to a class the same way that we initialize those member variables. This can be useful when we want to change the value a variable takes on based on something that happens inside of a class method.



**설명:** [ Learn ]      
• Ch8. Modifying member variables 에서는 클래스 변수를 수정하는 방법을 학습한다.     
• member 변수의 수정    
• 클래스 내부의 member 변수를 수정해서 사용할 필요가 있을때 변경할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside the `Car` class, add a method `drive_car` that sets `self.condition` to the string "used".

* Remove the call to `my_car.display_car()` and instead print only the `condition` of your car.

* Then drive your car by calling the `drive_car` method.

* Finally, print the `condition` of your car again to see how its value changes.  


**설명:** [ Instruction ]    
• 클래스 Car 내부에 메서드 drive_car() 를 만들어라.    
• 메서드 drive_car() 내부에 self.condition = "used" 을 만들어라.    
• my_car.display_car() 를 삭제 하여라.     
• 대신에 my_car.condition 값을 출력하라.    
• my_car.drive_car() 를 호출하라.    
• my_car.condition 을 출력하라.    
• condition 값이 어떻게 변했는지 살펴 보아라.
{: .notice--info}


<p style="page-break-before: always;"></p>
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
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg
   
  def display_car(self):
    print "This is a %s %s with %s MPG." % (self.color, self.model, str(self.mpg))
    
  def drive_car(self):
    self.condition = "used"

my_car = Car("DeLorean", "silver", 88)

print my_car.condition
my_car.drive_car()
print my_car.condition
```

**설명:** [ Solution ]     
• 클래스 내부에서 처음 정의한 condition 값은 "new" 이었다.    
• 메서드 drive_car() 가 호출되어 그 내부에 재정의한 condition 값은 "used" 이다.    
• member 변수 condition 값이 "new" 에서 "used"로 변경 되었다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>


**결과**     
```
new
used
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 9. Inheritance    

One of the benefits of classes is that we can create more complicated classes that inherit variables or methods from their parent classes. This saves us time and helps us build more complicated objects, since these child classes can also include additional variables or methods.

We define a "child" class that inherits all of the variables and functions from its "parent" class like so:
```python
class ChildClass(ParentClass):
  # new variables and functions go here
```
Normally we use object as the parent class because it is the most basic type of class, but by specifying a different class, we can inherit more complicated functionality.



**설명:** [ Learn ]      
• Ch9. Inheritance 에서는 상속(Inheritance)를 학습한다.     
• Inheritance(상속)    
• 클래스의 가장 유용한 점은 inheritance 를 할 수 있다는 것이다.    
• Inheritance 는 상위 클래스의 변수와 메소드를 상속 받을 수 있다.     
• 상속 받은 하위 클래스는 상위 클래스의 변수와 메소드 외에도 더 추가 할수가 있다.    
• 상위 클래스는 부모 클래스라고 부르고, 하위 클래스는 자식 클래스라고 한다.   
• 부모 클래스는 대부분 object 를 부모 클래스로 두고 있다.    
• 이런 inheritance 로 우리는 다양하고 복잡한 클래스를 만들수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a class `ElectricCar` that inherits from `Car`.     

<p style="page-break-before: always;"></p>
<br>

* Give your new class an `__init__()` method of that includes a `battery_type` member variable in addition to the `model`, `color` and `mpg`.

* Then, create an electric car named `my_car` with a "molten salt" battery_type.     
* Supply values of your choice for the other three inputs (model, color and mpg).  


**설명:** [ Instruction ]    
• 클래스 Car 를 inheritance 하는 클래스 ElectricCar 를 만들어라.    
• 클래스 ElectricCar 의 메서드 `__init__()` 내부에 member 변수 battery_type 를 추가하라.    
• my_car = ElectricCar("molten salt", model, color, mpg)를 만들어라.     
• model, color, mpg 에 당신이 원하는 값을 넣어라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Redefining a method of a "child" class is as simple as including a definition for that function inside the "child" class; this version will take precedence over the inherited version.

* Remember to include the self keyword as the first input when you define the `__init__()` method!


**설명:** [ Hint ]     
• 자식 클래스는 ( ) 안에 부모 클래스 이름을 적는다.    
• 자식 클래스의 `__init__()` 에 self 를 넣는것을 잊지 말자.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

<p style="page-break-before: always;"></p>
<br>


```python
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg
   
  def display_car(self):
    print "This is a %s %s with %s MPG." % (self.color, self.model, str(self.mpg))
    
  def drive_car(self):
    self.condition = "used"
    
class ElectricCar(Car):
  def __init__(self, model, color, mpg, battery_type):
    self.model = model
    self.color = color
    self.mpg   = mpg
    self.battery_type = battery_type

my_car = ElectricCar("DeLorean", "silver", 88, "molten salt")
```

**설명:** [ Solution ]     
• 클래스 ElectricCar 는 부모 클래스 Car를 inheritance 한다.    
• 입력 받은 파라미터들을 초기화 한다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 10. Overriding methods    

Since our `ElectricCar` is a more specialized type of `Car`, we can give the `ElectricCar` its own `drive_car()` method that has different functionality than the original `Car` class's.



**설명:** [ Learn ]      
• Ch10. Overriding methods 에서는 오버리이딩을 학습한다.   
• 클래스 ElectricCar 는 부모 클래스 Car 의 특화된 클래스이다.    
• 클래스 ElectricCar 의 내부 메서드 drive_car() 는 클래스 Car 내부의 메소드 drive_car() 와 다른 기능을 수행할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside `ElectricCar` add a new method `drive_car` that changes the car's `condition` to the string "like new".

* Then, outside of `ElectricCar`, print the `condition` of `my_car`

* Next, drive `my_car` by calling the `drive_car` function

* Finally, print the `condition` of `my_car` again

 
**설명:** [ Instruction ]    
• 클래스 ElectricCar 의 내부 메서드 drive_car() 의 member 변수 condition = "like new" 라고 추가한다.    
• 클래스 외부에, my_car = ElectricCar() 한 my_car.condition 을 출력한다.    
• my_car.drive_car() 를 호출한다.    
• my_car.condition 을 출력한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* This should be very similar to what you did in the second exercise of this section.


**설명:** [ Hint ]     
• 앞장에서 배운 override 예제를 참조 하시오.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Car(object):
  condition = "new"
  def __init__(self, model, color, mpg):
    self.model = model
    self.color = color
    self.mpg   = mpg
   
  def display_car(self):
    print "This is a %s %s with %s MPG." % (self.color, self.model, str(self.mpg))
    
  def drive_car(self):
    self.condition = "used"
    
class ElectricCar(Car):
  def __init__(self, model, color, mpg, battery_type):
    self.model = model
    self.color = color
    self.mpg   = mpg
    self.battery_type = battery_type
    
  def drive_car(self):
    self.condition = "like new"
```
<p style="page-break-before: always;"></p>
<br>

```python
my_car = ElectricCar("DeLorean", "silver", 88, "molten salt")

print my_car.condition
my_car.drive_car()
print my_car.condition
```

**설명:** [ Solution ]     
• 첫번째, print my_car.condition 은 "new"가 출력된다.     
• my_car.drive_car() 를 호출하면 기존 클래스가 아닌, ElectriCar에서 재정의한 drive_Car() 가 호출되면서, override 가 된다.    
• 다시, print my_car.condition 을 호출하면 "like new" 가 출력된다.
{: .notice--info}



**결과**     
``` 
new
like new
```     
<p style="page-break-before: always;"></p>
<br>

![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 11. Building useful classes    

Chances are, you won't be designing `Car` classes in the real world anytime soon. Usually, classes are most useful for holding and accessing abstract collections of data.

One useful class method to override is the built-in `__repr__()` method, which is short for representation; by providing a return value in this method, we can tell Python how to represent an object of our class (for instance, when using a print statement).



**설명:** [ Learn ]       
• Ch11. Building useful classes 에서는 클래스를 연습한다.    
• 실전 프로그램에서, 클래스는 유용하게 사용된다.     
• 하지만, 여러분이 바로 클래스를 만들고 사용하는 일은 조금 시간이 걸린다.   
• 이렇게 유용한 클래스를 잘 사용하게끔 하려고, 새로운 내장 메서드가 있다.    
• 이 내장 메서드는 따로 구현할 필요 없이 overriding 기능을 활용하여 쉽게 사용할수 있게 해준다.    
• 지금 소개할 대표적 메서드는 `__repr__()` 이다.    
• 이 메서드는 Python에서 객체를 반환할때, 어떻게 표현할지를 정확하게 알려주는 메서드이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a `Point3D` class that inherits from `object`

* Inside the `Point3D` class, define an `__init__()` function that accepts `self`, `x`, `y`, and `z`, and assigns these numbers to the member variables `self.x`, `self.y`, `self.z`

* Define a `__repr__()` method that returns "(%d, %d, %d)" % (self.x, self.y, self.z).     


* This tells Python to represent this `object` in the following format:    
     
```python
(x, y, z).
```

<p style="page-break-before: always;"></p>
<br>

* Outside the class definition, create a variable named `my_point` containing a new instance of `Point3D` with `x=1`, `y=2`, and `z=3`.

* Finally, print `my_point`.


**설명:** [ Instruction ]    
• `__repr__()` 의 개념을 익히기 위하여 연습해 보자.    
• 클래스 Point3D(object) 를 작성하라.    
• 클래스 Point3D는 메서드 `__init__()` 를 가진다.    
• 메서드 `__init__()` 는 parameter 로 self, x, y, z 를 가진다.    
• 그리고, 각 변수 x, y, z 를 초기화 한다. (e.g. self.x )    
• 클래스 Point3D 에 메서드 `__repr__()` 를 추가한다.    
• 메서드 `__repr__()` 는 다음과 같이 변환한다.    
• e.g. "(%d, %d, %d)" % (self.x, self.y, self.z)    
• 출력시 ( x, y, z ) 로 출력이 된다.     
• 외부에서 my_point = Point3D(1, 2, 3) 이라고 호출한다.    
• my_point 를 출력하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* When defining a new `__repr__()`, return a string value that uses the member variables of the class to display the 3D point properly.     
* You can use the `str()` function to put these numbers in the proper string.

* For advanced users: For more information on `__repr__` and other special methods see this Python documentation. Note the slight difference between the `__repr__` and `__str__` methods.

```python
# x=1, y=2, z=3
my_point = point3D(1,2,3)
```
**설명:** [ Hint ]     
• `__repr__()` 를 사용할때는 문자열이 반환된다.    
• 반환할때, 숫자는 `str()` 를 사용하여 반환하라.    
• `__repr__` 이외의 다른 특별한 메서드에 대해서 궁금하면 Python 매뉴얼을 참조하라.    
• `__repr__` 과 `__str__` 사이의 약간의 차이점도 알아보자.      
• `__repr__` 는 정확하게 내가 표현할때 사용한다.    
• `__str__` 은 Python이 제공하는 기능을 참조하여 정해진 기본값을 보여줄때, 사용한다.
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>

• 소숫점 20자리의 결과 값을 보여줄때, `__repr__`는 정확히 20자리를 보여줄수 있다.    
• 하지만, `__str__` 은 Python 해석기가 기본으로 보여줄수 있는 적당한 값 (15자리 or 그보다도 적거나 많을수도 있음)을 보여준다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
class Point3D(object):
  def __init__(self, x, y, z):
    self.x = x
    self.y = y
    self.z = z
    
  def __repr__(self):
    return "(%d, %d, %d)" % (self.x, self.y, self.z)
    
my_point = Point3D(1, 2, 3)
print my_point
```

**설명:** [ Solution ]     
• `__repr__(self)` 는 내가 object 에서 호출시 정확히 보여주고자 하는 결과값을 출력해 준다.
{: .notice--info}



**결과**     
``` 
(1,2,3)
```   