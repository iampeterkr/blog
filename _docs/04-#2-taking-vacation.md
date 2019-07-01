---
# layout : rchive
title: "Taking A Vacation"
permalink: /taking-vacation/
excerpt: "We learn about Funcations."
# last_modified_at: 2019-02-09T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---


<hr style="border: solid 1px #dddddd ;">    

LESSON    

Hard day at work? Rough day at school? Take a load off with a programming vacation!    


**설명:** [ 학습방향 ]     
이 장에서는 여행의 경비를 계산해주는 함수를 만들어 보면서, 관련 함수를 만드는 연습을 통하여 함수에 대한 개념과 사용법에 대하여 익숙해지자.
{: .notice--info}     
     

    
<hr style="border: solid 1px #dddddd ;">    
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 1. Before We Begin   

Let's first quickly review functions in Python.
<br>
```python
def bigger(first, second):
  print max(first, second)
  return True   
```
<br>
In the example above:

* We define a function called `bigger` that has two arguments called `first` and `second`.   

* Then, we print out the larger of the two arguments using the built-in function `max`.    

* Finally, the `bigger` function returns True.    

* Now try creating a function yourself!

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Learn ]    
• Ch1. Before We Begin 는 내장함수(built-in) max() 를 학습한다.    
• 함수 bigger() 는 arguments 값으로 first 와 second 를 가진다.    
• 그리고 built-in 함수인 max() 사용하여 first 와 second 두 값을 비교한다.    
• 함수 max() 는 두 값을 비교하여 큰 값을 출력한다.    
• 정상적 동작을 완료하면, 함수는 True 값을 반환한다.    
• 지금부터 각자의 함수를 만들어 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write a function called `answer` that takes no arguments and returns the value `42`.

* Even without arguments, you will still need parentheses. Don't forget the colon at the end of the function definition!


**설명:** [ Instruction ]     
• 함수 answer() 를 만들어라.    
• 함수 answer() 는 값 42 를 반환한다.    
• 주의 사항은 함수끝에 ( : ) 를 잊지말자.
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
def answer():
  return 42
```

**설명:** [ Solution ]    
• ( : ) 를 주의한다.  
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 2.  Planning Your Trip    

When planning a vacation, it's very important to know exactly how much you're going to spend.

``` python
def wages(hours):
  # If I make $8.35/hour...
  return 8.35 * hours
```     

The above example is just a refresher in how functions are defined.

Let's use functions to calculate your trip's costs.


**설명:** [ Learn ]    
• Ch2. Planning Your Trip 에서는 함수 wages() 를 학습한다.    
• 예상 여행비용을 계산해주는 프로그램을 만든다고 가정해 보자.     
• 여행 비용을 계산해주는 함수 wages() 를 위와 같이 만들수 있다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Define a function called `hotel_cost` with one argument `nights` as input.

* The hotel costs `$140` per night. So, the function `hotel_cost` should return `140 * nights`.


**설명:** [ Instruction ]    
• 함수 hotel_cost() 를 만들어라.    
• 함수 hotel_const(nights)는 arguments 값으로 nights 를 가진다.    
• 함수 hotel_cost(nights)는 1박당 $140 로 계산한다.    
• 함수 hotel_cost(nights)는 nights x $140 로 비용을 계산한다.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)

* Your function should return the number of `nights`you stay multiplied by 140.    


**설명:** [ Hint ]     
• 1박당 $140 로 계산하여, nights x 140 을 곱하여 계산한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights
```

**설명:** [ Solution ]     
• nights 는 박수를 의미하며, 140 은 1박당 비용이다.     
• 함수 hotel_cost(nights)는 총 비용을 반환한다.
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
<font size="3"  face="돋움">TAKING A VACATION</font>    

### 3. Getting There    

You're going to need to take a plane ride to get to your location.

<br>

```python
def fruit_color(fruit):
  if fruit == "apple":
    return "red"
  elif fruit == "banana":
    return "yellow"
  elif fruit == "pear":
    return "green"
```

* The example above defines the function `fruit_color` that accepts a string as the argument `fruit`.    

* The function returns a string if it knows the color of that fruit.


**설명:** [ Learn ]    
• Ch3. Getting There 에서는 함수내에 if / elif / else 조건절 사용을 학습한다.      
• 함수 fruit_color(fruit) 는 문자열 타입의 arguments 값인 fruit 를 입력받는다.    
• 입력받은 fruit 와 일치하는 문자열을 찾아서, 색깔 문자열을 반환한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your existing code, define a function called `plane_ride_cost` that takes a string, `city`, as input.
<p style="page-break-before: always;"></p>
<br>

* The function should return a different price depending on the location, similar to the code example above. Below are the valid destinations and their corresponding round-trip prices.

  * "Charlotte": 183
  * "Tampa": 220
  * "Pittsburgh": 222
  * "Los Angeles": 475



**설명:** [ Instruction ]    
• 함수 plane_ride_cost(city) 는 arguments city 에 따라 반환하는 값이 틀려진다.    
• city 입력값이 도시명 "Charlotte" 이면 왕복 비행기 값 183 을 반환한다.    
• city 입력값이 도시명 "Tampa"     이면 왕복 비행기 값 220 을 반환한다.    
• city 입력값이 도시명 "Charlotte" 이면 왕복 비행기 값 183 을 반환한다.    
• city 입력값이 도시명 "Los Angeles" 이면 왕복 비행기 값 475 을 반환한다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You could use if/elif/else to return the price that's appropriate to the function's input.    



**설명:** [ Hint ]    
• if / elif / else 를 사용하라.    
• 기존 함수 hotel_cost() 는 놔두고, 그 밑에 새로운 함수를 작성하라. 
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights

def plane_ride_cost(city):
  if city == "Charlotte":
    return 183
  elif city == "Tampa":
    return 220
  elif city == "Pittsburgh":
    return 222
  elif city == "Los Angeles":
    return 475
```

**설명:** [ Solution ]    
• 함수 plane_ride_cost(city) 는 입력된 도시명에 따라 비용이 각각 계산된다.
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 4. Transportation    

You're also going to need a rental car in order for you to get around.

```python
def finish_game(score):
  tickets = 10 * score
  if score >= 10:
    tickets += 50
  elif score >= 7:
    tickets += 20
  return tickets
```

In the above example, we first give the player 10 tickets for every point that the player scored. Then, we check the value of score multiple times.

* First, we check if score is greater than or equal to `10`. If it is, we give the player `50` bonus tickets.    

* If score is just greater than or equal to `7`, we give the player `20` bonus tickets.    

* At the end, we return the total number of tickets earned by the player.    

* Remember that an `elif` statement is only checked if all preceding `if/elif` statements fail.


**설명:** [ Learn ]    
• Ch4. Transportation 에서는 또 다른 함수 finish_game() 를 만들어 보자.     
• 상기 함수는 점수 당 티켓 10 장을 주는 함수이다.    
• 입력된 source 점수가 10 이상 이면 보너스로 티켓을 50 장 더 지급한다.    
• 입력된 source 점수가  7 이상 & 10 미만이면, 보너스로 티켓을 20 장 더 지급한다.    
• 최종적으로 전체 티켓수를 반환한다.     
• elif 문은 if 문이 실패하면 elif 문을 실행된다.   
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your existing code, define a function called `rental_car_cost` with an argument called `days`.

* Calculate the cost of renting the car:

* Every day you rent the car costs `$40`.    

* if you rent the car for `7` or more days, you get `$50` off your total.    

* *Alternatively* (elif), if you rent the car for `3` or more days, you get `$20` off your total.    

* You cannot get both of the above discounts.
Return that cost.    

* Just like in the example above, this check becomes simpler `if` you make the 7-day check an if statement and the 3-day check an `elif` statement.


**설명:** [ Instruction ]    
• 함수 rental_car_cost(days) 를 만들어라.    
• 이 함수는 차 렌트 비용을 계산해준다.   
• 1일 렌트 비용은 $40 이다.     
• 7일 이상 렌트시 총 비용에서 $50 를 할인해 준다.    
• 3일 이상 7일 미만 렌트시 총 비용에서 $20 를 할인해 준다.    
• 2 가지 혜택중 하나만 선택할 수 있다.     
• 프로그램 구현시, $50 할인은 if 문을 사용하라.    
• $ 30 할인은 elif 문을 사용하여 구현하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Remember to use an `elif` so you don't subtract both of the discounts! (You'll want to do your check for >= 7 days first.)    

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]    
• 7 일 이상 확인하는것을 먼저 if 문에 넣어야 한다.      
• if 문에 3 일 이상을 먼저 비교하면, 어떤 문제점이 있는지도 생각해 보자. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights

def plane_ride_cost(city):
  if city == "Charlotte":
    return 183
  elif city == "Tampa":
    return 220
  elif city == "Pittsburgh":
    return 222
  elif city == "Los Angeles":
    return 475

def rental_car_cost(days):
  cost = days * 40
  if days >= 7:
    cost -= 50
  elif days >= 3:
    cost -= 20
  return cost
```

**설명:** [ Solution ]     
• 만약 ( if cost >= 3 )을 먼저 비교문을 만들게 되면 다음 상황이 발생하게 된다.         
• 변수 cost 에 8 이 들어온다고 가정하면,     
• ( if cost >= 3 )도 만족하고, ( elif cost >= 7 )도 만족하게 된다.    
• 이렇게 되면 2번 할인이 일어 나기에 조심해야 한다.    
• 그렇기에, ( if cost >= 7 )을 먼저 비교하고, ( elif cost >= 3 )을 비교한다.
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 5. Pull it Together    

Great! Now that you've got your 3 main costs figured out, let's put them together in order to find the total cost of your trip.

<br>

```python
def double(n):
  return 2 * n

def triple(p):
  return 3 * p

def add(a, b):
  return double(a) + triple(b)
```
<br>

We define two simple functions, `double(n)` and `triple(p)` that return 2 times or 3 times their input. Notice that they have `n` and `p` as their arguments

We define a third function, `add(a, b)` that returns the sum of the previous two functions when called with `a` and `b`, respectively. Notice that even though the names of the parameters for `add(a, b)` are different than the names of the parameters for `double(n)` and `triple(p)` we can still pass them into those functions as arguments

<br>

**설명:** [ Learn ]    
• Ch5. Pull it Together 에서는 함수에서 함수를 호출하는것을 학습한다.    
• 함수는 arguments 를 1개 이상을 받을 수 있다.    
• 함수는 반환(return) 할때, 변수를 계산할 수 있다.    
• 함수는 반환(return) 할때, 함수를 호출할 수 있다. 
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Below your existing code, define a function called `trip_cost` that takes two parameters, `city` and `days` and returns the sum of calling the `rental_car_cost(days)`, `hotel_cost(days - 1)`, and `plane_ride_cost(city)` functions.

* Notice that we changed the argument of `hotel_costs()` from nights to days - 1. Since we want trip-cost to only depend on two parameters, we have to convert the variable nights into days. If you are going to be staying somewhere, the number of nights you stay there is one less than the number of days you were there (imagine a weekend trip to visit family, you leave Saturday and return Sunday, so you visit for two days, but only stay for one night).

<br>

**설명:** [ Instruction ]    
• 함수 trip_cost() 를 정의하여라.     
• 함수 trip_cost(city, day) 는 2 개의 parameters 를 가진다.    
• 함수 trip_cost(city, day) 는 함수 ① retal_car_cost(days) 를 호출한다.    
• 함수 trip_cost(city, day) 는 함수 ② hotel_cost(days - 1) 를 호출한다.    
• 함수 trip_cost(city, day) 는 함수 ③ plane_ride_cost(city)를 호출한다.    
• 함수 trip_cost(city, day) 는 함수 ①,②,③ 의 합을 반환(return) 한다.    
• 단, 함수 ② hotel_cost(days - 1) 의 기능인 1박을 제외하는것을 유의하라.
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
def hotel_cost(nights):
  return 140 * nights

def plane_ride_cost(city):
  if city == "Charlotte":
    return 183
  elif city == "Tampa":
    return 220
  elif city == "Pittsburgh":
    return 222
  elif city == "Los Angeles":
    return 475

def rental_car_cost(days):
  cost = days * 40
  if days >= 7:
    cost -= 50
  elif days >= 3:
    cost -= 20
  return cost

def trip_cost(city, days):
  return rental_car_cost(days) + hotel_cost(days - 1) + plane_ride_cost(city)
```

**설명:** [ Solution ]    
• 함수 trip_cost(city, days) 는 return 문에서 바로 함수를 호출한다.    
• 호출한 함수의 결과를 합하여 반환한다.
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 6. Hey, You Never Know!
You can't expect to only spend money on the plane ride, hotel, and rental car when going on a vacation. There also needs to be room for additional costs like fancy food or souvenirs.


**설명:** [ Learn ]   
• Ch6. Hey, You Never Know! 에서는 기존 함수에 parameter를 추가를 학습한다.        
• 프로그램을 더 추가해 보자.    
• 음식값, 기년품 값등 추가로 사용한 비용을 계산해 주는 기능도 추가해 볼 수 있다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Modify your `trip_cost` function definition. Add a third argument, `spending_money`.

* Modify what the `trip_cost` function does. Add the variable `spending_money` to the sum that it returns.


**설명:** [ Instruction ]    
• 함수 trip_cost() 에 3번째 parameter 변수 spending_money 를 추가하라.    
• 함수 trip_cost() 에 변수 spending_money 의 값을 전체 값에 추가하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Add to return variables `spending_money`. 

<p style="page-break-before: always;"></p>
<br>

**설명:** [ Hint ]    
• return 문에서 합을 구할때, 변수 spending_money 를 추가하라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights

def plane_ride_cost(city):
  if city == "Charlotte":
    return 183
  elif city == "Tampa":
    return 220
  elif city == "Pittsburgh":
    return 222
  elif city == "Los Angeles":
    return 475

def rental_car_cost(days):
  cost = days * 40
  if days >= 7:
    cost -= 50
  elif days >= 3:
    cost -= 20
  return cost

def trip_cost(city, days, spending_money):
  return rental_car_cost(days) + hotel_cost(days) + plane_ride_cost(city) + spending_money
```

**설명:** [ Solution ]    
• 기존 함수 trip_cost() 에 parameter 변수 spending_money 를 추가하였다.    
• e.g. def trip_cost(city, days, spending_money):          
• 함수 trip_cost() 의 반환(return)문에 변수 spending_money 값을 추가하였다.
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
<font size="3"  face="돋움">TAKING A VACATION</font> 

### 7. Plan Your Trip!    

Nice work! Now that you have it all together, let's take a trip.

What if we went to Los Angeles for 5 days and brought an extra 600 dollars of spending money?


**설명:** [ Learn ]    
• Ch7. Plan Your Trip! 에서는 지금껏 만든 함수를 trip_cost() 호출후 출력해보자.    
• 함수를 호출할때, arguments 는 다음 내용을 생각해 보자.     
• 로스엔젤레스 에서 5일 머무르고,    
• 추가 비용으로 600 달러를 사용하면 여행비용은 얼마일까?
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* After your previous code, print out the `trip_cost`( to "Los Angeles" for 5 days with an extra 600 dollars of spending money.

* Don't forget the closing ) after passing in the 3 previous values!


**설명:** [ Instruction ]    
• 함수 trip_cost() 를 호출하라.    
• 입력시, arguments 값은 다음과 같다.    
• city : "Los Angeles"    
• days : 5 일    
• spending_money : $ 600    
• 함수 trip_cost()에 위 값을 입력하여 호출하라.
{: .notice--info}


<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* You'll want to `print` the result of calling `trip_cost` with the above values as arguments!

* Your final call should look something like:    

```python
print trip_cost("SOME CITY", NUM_DAYS, SPENDING_MONEY)
```    

* where SOME CITY is one of the four cities, NUM_DAYS is the number of days and SPENDING_MONEY is the amount of spending money.    

**설명:** [ Hint ]    
• 함수 trip_cost(city, days, spending_money) 와 같이 입력값을 가진다.     
• 함수 arguments 값에 직접 값을 넣어서 함수를 호출하라.    
• 함수를 호출하고, 그 결과값을 보기 위해선, print 문을 사용해야 한다.     
• e.g. print trip_cost("LA", 7, 1000)
{: .notice--info}

<p style="page-break-before: always;"></p>
<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights

def plane_ride_cost(city):
  if city == "Charlotte":
    return 183
  elif city == "Tampa":
    return 220
  elif city == "Pittsburgh":
    return 222
  elif city == "Los Angeles":
    return 475

def rental_car_cost(days):
  cost = days * 40
  if days >= 7:
    cost -= 50
  elif days >= 3:
    cost -= 20
  return cost

def trip_cost(city, days, spending_money):
  return rental_car_cost(days) + hotel_cost(days) + plane_ride_cost(city) + spending_money

print trip_cost("Los Angeles", 5, 600)
```

**설명:** [ Solution ]    
• 함수 trip_cost()의 arguments 값으로 "Lost Angelse", 5, 600 을 직접 입력하였다.    
• print 문을 사용하여 함수 trip_cost()의 결과값을 출력하였다.
{: .notice--info}



**결과** 
```
1955 
```