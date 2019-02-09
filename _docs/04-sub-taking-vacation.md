---
# layout : rchive
title: "Taking A Vacation"
permalink: /taking-vacation/
excerpt: "We learn about Funcations."
last_modified_at: 2019-02-09T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---

<hr style="border: solid 1px #dddddd ;">    

LESSON    

Hard day at work? Rough day at school? Take a load off with a programming vacation!    


**설명:** [ 학습방향 ]     
함수에 대해서 좀 더 연습해 보자.
{: .notice--info}     
     

    
<hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 1. Before We Begin   
Let's first quickly review functions in Python.

```python
def bigger(first, second):
  print max(first, second)
  return True   
```
In the example above:

① We define a function called `bigger` that has two arguments called `first` and `second`.   
② Then, we print out the larger of the two arguments using the **built-in function** `max`.
Finally, the `bigger` function returns **True**.   
③ Now try creating a function yourself!


**설명:** [ ]      [ ]      함수 `bigger` 는 `first` 와 `second` 2개의 argument를 가진다. 그리고 built-in 함수인 `max` 사용하여 `first`와 `second` 두 값을 비교하여 큰값을 출력하며, True 값을 Return 한다. 지금부터 각자의 함수를 만들어 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function called `answer` that takes **no arguments** and returns the value `42`.

Even without arguments, you will still need **parentheses**. Don't forget the **colon** at the end of the function definition!


**설명:** [ ]      ① 함수 `answer()`를 만들고, 이 함수는 `42`를 return 한다. 주의사항은 함수에 `()` 와 `:`를 잊지 말아야 한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)skip    



**설명:** [ ]      skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def answer():
  return 42
```

**설명:** [ ]      `()`, `:` 를 주의한다.  
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


**설명:** [ ]      여행중 예상되는 비용을 계산해주는 프로그램을 짠다고 가정해 보자. 여행 비용을 계산해주는 함수 `wages`를 위와 같이 만들수 있다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called `hotel_cost` with **one argument** `nights` as input.

The hotel costs `$140` per night. So, the function `hotel_cost` should return `140 * nights`.


**설명:** [ ]      ① 함수 `hotel_cost()`를 만들자. 이 함수는 `nights` input arguments를 가진다. `hotel_cost()`함수는 1박당 `$140`으로 쳐서, 총 박수 x 1박 비용을 계산해 준다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)Your function should **return** the number of `nights`you stay **multiplied** by **140**.    


**설명:** [ ]      1박당 140을 곱하여 계산한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def hotel_cost(nights):
  return 140 * nights
```

**설명:** [ ]      `nights` 는 박수를 의미하며, `140`은 1박당 비용이다. 
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 3.  Getting There
You're going to need to take a plane ride to get to your location.

```python
def fruit_color(fruit):
  if fruit == "apple":
    return "red"
  elif fruit == "banana":
    return "yellow"
  elif fruit == "pear":
    return "green"
```

① The example above defines the function `fruit_color` that accepts a **string** as the **argument** `fruit`.    

② The function **returns** a **string** if it knows the color of that fruit.


**설명:** [ ]      함수 `fruit_color()`는 문자열 타입의 argument `fruit` 를 입력받아, 그와 일치하는 값을 반환하는 함수이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①**  Below your existing code, define a function called `plane_ride_cost` that takes a **string**, `city`, as **input**.

The function should return a different price depending on the location, similar to the code example above. Below are the valid destinations and their corresponding round-trip prices.

* "Charlotte": 183
* "Tampa": 220
* "Pittsburgh": 222
* "Los Angeles": 475



**설명:** [ ]      ① 함수 `plane_ride_cost()`는 입력값 `city`에 따라 반환하는 값이 틀려진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You could use if/elif/else to return the price that's appropriate to the function's input.    



**설명:** [ ]      `if/elif/else`를 사용하여라. 기존 함수 `hotel_cost()`는 놔두고, 그 밑에 새로운 함수를 만들어라. 
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
```

**설명:** [ ]      함수 `plane_ride_cost(city)`는 입력된 도시명에 따라 각 비용이 각각 계산된다.
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

① First, we check if score is **greater than** or **equal** to `10`. If it is, we give the player `50` **bonus** tickets.    

② If score is just **greater than** or **equal** to `7`, we give the player `20` **bonus** tickets.    

③ At the end, we return the total number of tickets earned by the player.
Remember that an `elif` statement is only checked if all preceding `if/elif` statements fail.


**설명:** [ ]      ① 입력된 `bonus` 점수가  `10` 이상이면 보너스로 티켓을 50장 더주고, 
② 점수가 `7`이상이면, 보너스로 티켓을 20장 더주는 역할을 하는 함수이다.  
③ 최종적으로 전체 티켓 수를 반환한다. `elif`문은 `if`문이 실패하면 다음을 점검한다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Below your existing code, define a function called `rental_car_cost` with an argument called `days`.

Calculate the cost of **renting** the car:

* Every day you rent the car costs `$40`.
* if you rent the car for `7` or **more days**, you get `$50` **off** your total.
* *Alternatively* (elif), if you rent the car for `3` or **more days**, you get `$20` **off** your total.
* You **cannot** get **both** of the above **discounts**.
Return that cost.

Just like in the example above, this check becomes simpler `if` you make the **7-day** check an if statement and the **3-day** check an `elif` statement.


**설명:** [ ]      ① 함수 `rental_car_cost(days)`를 만들어라. 
* 1일 렌트비용은 `$140`이다. 
* 7일 이상 렌트시 총 비용에서 `$50`를 할인해 주고,
* 3일 이상 렌트시 총 비용에서 `$20`를 할인해 준다. 
* 2가지 모두 혜택을 받을수는 없고, 프로그램 구현시, `$50`는 `if`문을 사용하고, `30`은 `elif`문을 사용하여 구현하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)Remember to use an `elif` so you don't subtract both of the discounts! (You'll want to do your check for >= 7 days first.)    

**설명:** [ ]      `7`일 이상을 먼저 `if`문에 넣어야 한다.  `if`문에 `3`일을 먼저 check하면 어떤일이 벌얼질지 생각해 보자. 
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

**설명:** [ ]      만약 `>=3`을 먼저 저검하면, `elif`에서 `=>7`도 점검되어 이중 할인이 일어나게 된다. 그 부분을 조심하자.  
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 5. Pull it Together
Great! Now that you've got your **3 main costs** figured out, let's put them together in order to find the **total cost** of **your trip**.

```python
def double(n):
  return 2 * n

def triple(p):
  return 3 * p

def add(a, b):
  return double(a) + triple(b)
```

We define two simple functions, `double(n)` and `triple(p)` that return 2 times or 3 times their input. Notice that they have `n` and `p` as their arguments

We define a third function, `add(a, b)` that returns the sum of the previous two functions when called with `a` and `b`, respectively. Notice that even though the names of the parameters for `add(a, b)` are different than the names of the parameters for `double(n)` and `triple(p)` we can still pass them into those functions as arguments

**설명:** [ ]      arguments 를 1개도 받을수 있고, 2개도 받을수 있다. 함수에서 또 함수를 호출 할수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Below your existing code, define a function called `trip_cost` that takes **two parameters**, `city` and `days` and **returns** the sum of calling the `rental_car_cost(days)`, `hotel_cost(days - 1)`, and `plane_ride_cost(city)` functions.

**Notice** that we changed the argument of `hotel_costs()` from nights to **days - 1**. Since we want trip-cost to only depend on two parameters, we have to convert the variable nights into days. If you are going to be staying somewhere, the number of nights you stay there is one less than the number of days you were there (imagine a weekend trip to visit family, you leave Saturday and return Sunday, so you visit for two days, but only stay for one night).


**설명:** [ ]      ① 함수 `trip_cost()`를 정의하여라. ② 이 함수는 `city`, `day` 입력값을 가지며 ③ `retal_car_cost(days)`, `hotel_cost(days - 1)`를 호출하여 계산된 총합을 반환한다. ④ `hotel_cost(days - 1)`함수에서 1박을 제외하는것을 유의하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
`hotel_cost(days - 1)`을 주의하라. 
return 에서 바로 함수를 호출하여 `+` 를 사용하여 계산하라.



**설명:** [ ]      호텔 비용을 계산할때는 1박을 제외해야 한다. return 에서 `+`를 사용하여 바로 계산하라. 
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

def trip_cost(city, days):
  return rental_car_cost(days) + hotel_cost(days - 1) + plane_ride_cost(city)
```

**설명:** [ ]      return 문에서 바로 함수를 호출하여 사용한후, 바로 반환한다.
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 6. Hey, You Never Know!
You can't expect to only spend money on the plane ride, hotel, and rental car when going on a vacation. There also needs to be room for additional costs like fancy food or souvenirs.


**설명:** [ ]      추가적인 음식값이나, 기년품값을 추가가 필요 할수도 있다. 프로그램을 더 추가해 보자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** **Modify** your `trip_cost` function definition. **Add** a third argument, `spending_money`.

**Modify** what the `trip_cost` function does. Add the variable `spending_money` to the sum that it returns.


**설명:** [ ]      ① 함수 `trip_cost()`에 3번째 입력값 `spending_money`를 추가하라. ② 함수 내부 기능에 `spending_money`의 값을 전체 값에 추가하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Add to return variables `spending_money`. 


**설명:** [ ]      return 문에 `spending_money`를 추가하라.  
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

**설명:** [ ]      return 문에 `spending_money`를 추가한다. 
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
<font size="3"  face="돋움">TAKING A VACATION</font> 
### 7. Plan Your Trip!
Nice work! Now that you have it all together, let's take a trip.

What if we went to Los Angeles for 5 days and brought an extra 600 dollars of spending money?


**설명:** [ ]      로스엔젤레스 에서 5일 머무르고, 600달러를 사용하면 어떨까?
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** After your previous code, **print out** the `trip_cost`( to "Los Angeles" for 5 days with an extra 600 dollars of spending money.

Don't forget the closing ) after passing in the 3 previous values!


**설명:** [ ]      ① 함수 `trip_cost()`를 호출할때, 입력값으로 도시 입력값에 "Los Angeles"를 입력하고 여행일자는 5일, 총 사용비용은 600 달러가 출력되게 하자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)You'll want to `print` the result of calling `trip_cost` with the above values as arguments!

Your final call should look something like:
```python
print trip_cost("SOME CITY", NUM_DAYS, SPENDING_MONEY)
```
where **SOME CITY** is one of the four cities, **NUM_DAYS** is the number of days and **SPENDING_MONEY** is the amount of spending money.    
**설명:** [ ]      `trip_cost(city, days, spending_money)`라고 함수를 정의해 놓았다. 각 입력값에 직접 값을 넣어서 호출한다.   
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

print trip_cost("Los Angeles", 5, 600)
```

**설명:** [ ]      정의된 함수를 호출하여 그 결과값이 반환되어 출력된다. 
{: .notice--info}



**결과** 
```
1955 
```

<br>
<br>    
<br>    

