---
# layout : rchive
title: "Classes"
permalink: /classes/
excerpt: "We learn about Classes Syntax."
last_modified_at: 2019-01-26T09:00:00-04:00
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

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">CLASSES</font> 
### 1.  Class basics    

Classes can be very useful for storing complicated objects with their own methods and variables. Defining a class is much like defining a function, but we use the class keyword instead. We also use the word object in parentheses because we want our classes to inherit the object class. This means that our class has all the properties of an object, which is the simplest, most basic class. Later we'll see that classes can inherit other, more complicated classes. An empty class would look like this:
```python
class ClassName(object):
  # class statements go here
```



**설명:** [ Learn ]     
• 클래스는 여러 가지 유용한 것들이 많다.    
• 메서드와 변수들이 섞여 있는 객체를 만드는데 유용하다.    
• 클래스간 Inherits(상속)를 할 수 있다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a new class named "Car".     
* For now, since we have to put something inside the class, use the `pass` keyword. 


**설명:** [ Instruction ]    
• 클래스  "Car"를 만들어라.    
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
• 클래스 Car는 object를 가진다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 2. Create an instance of a class    

We can use classes to create new **objects**, which we say are **instances** of those classes.

Creating a new instance of a class is as easy as saying:
```python
newObject = ClassName()
``` 


**설명:** [ Learn ]     
• 클래스를 사용하는 방법은 다음과 같다.    
• 클래스 ClassName() 를 instance 하는 object newObject 를 만든다.    
• newObject = ClassName()
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your `Car` class, create a new object named `my_car` that is an instance of `Car`. 


**설명:** [ Instruction ]    
• 클래스 Car 를 instance 하는 object my_car 를 만드시오.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Reference the description above, how to make new instance


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
skip
```   

<br>
<br>    
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
• member변수는 클래스 object 내부에 있는 변수이다.    
• member변수를 만들고 초기화 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Inside your `Car` class, replace the `pass` statement with a new member variable named `condition` and give it an initial value of the string "new". 


**설명:** [ Instruction ]    
• 클래스 Car 안에 있는 pass 를 지우시오.    
• 그 자리에 member 변수 condition을 만드시오.    
• 변수 condition을 초기화 하시오. (e.g. condition = "new")
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
class Car(object):
  condition = "new"

my_car = Car()
```

**설명:** [ Solution ]     
• member변수 condition에 초기값 "new"를 저장한다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 4. Calling class member variables    

Each class object we create has its own set of **member variables**. Since we've created an object `my_car` that is an instance of the `Car` class, `my_car` should already have a member variable named `condition`. This attribute gets assigned a value as soon as `my_car` is created.





**설명:** [ Learn ]      
• object my_car를 만들면, 클래스 에서 선언된 member변수 condition이 자동으로 할당된다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* At the end of your code, use a print statement to display the `condition` of `my_car`. 


**설명:** [ Instruction ]    
• object my_car의 member변수 condition을 출력하여라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Since the attribute condition belongs to the object `my_car`, you'll need to use **dot** notation to access the object's member variable: 
```python
my_car.condition.
```

**설명:** [ Hint ]     
• my_car.condition
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
• object my_car 의 member변수 condition을 호출하고 출력한다. 
{: .notice--info}



**결과**     
``` 
new
```   

<br>
<br>    
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
• 객체를 만들기 위해서 클래스를 호출하면, 해당 클래스의 `__init__()`이 호출된다.    
• 클래스 내에 있는 기본 `__init__()`를 우리가 추가 정의 할수도 있다.    
• `__init__(self)`첫번째, argument는 무조건 self 이다.    
• 객체가 self를 이용하여 자신을 추척한다.    
• `__init__(self, a, b,c)` self 이후에는 여러개의 변수를 전달할수 있다.    
•  클래스에 접근하기 위해선,  . 을 이용하여 접근이 가능 하다.    
• `__init__()`에 값이 전달되면 다음과 같이 메서드 내부에 값을 전달할수 있다.    
• self.new_variable = new_variable  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

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
• 메서드 `__init__()` 내부에 입력된 변수를 self를 이용하여 초기화 하여라.    
• 클래스 Car 를 instance 한 object my_car 를 아래 값들을 이용하여 수정하여라.    
• my_car = Car(model="DeLorean", color = "silver", mpg=88) 호출한다.    
• 참고로, object my_car를 생성할때, Car(self, a, b, c) self를 넣지 않는 이유는    
• 넣지 않아도, 자동으로 self가 입력된다.
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
```

**설명:** [ Solution ]     
• `__init__(self, model, color, mpg):` 변수 초기화는 다음과 같다.    
• e.g. self.model = model  
• my_car를 만들때, member변수 초기값("DeLorean", "silver", 88)을 넣는다.
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
<font size="3"  face="돋움">CLASSES</font> 
### 6.  



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 7. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 8. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 9. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 10. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 11. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 12. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 13.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 14. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 15.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 16. 



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 17.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 18.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
<font size="3"  face="돋움">CLASSES</font> 
### 19.



**설명:** [ Learn ]     
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

*  


**설명:** [ Instruction ]    
*  

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
