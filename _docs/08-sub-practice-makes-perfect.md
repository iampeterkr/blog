---
# layout : rchive
title: "Practice Makes Perfect"
permalink: /practice-makes-perfect/
excerpt: "We practice about loop."
last_modified_at: 2019-01-15T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 1. Practice! Practice Practice!    

The best way to get good at anything is a lot of practice. This lesson is full of practice problems for you to work on. Each exercise will contain minimal instructions to help you solve these problems. The goal is to help you take your programming skills and apply them to real life problems.

The more challenging programs will contain some helpful hints to nudge you in the right direction.

 



**설명:**     
프로그램을 잘 짜는 방법은 오직 연습뿐이다. loop를 배웠으니, 반복적으로 연습하면 프로그래밍 실력이 높아진다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Hit Run to continue.


**설명:**     
① `Run`을 클릭하여 다음으로 넘어가시오.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
skip


**설명:**     
skip
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
skip
```

**설명:**     
skip
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
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 2.  is_even    

All right! Let's get started.

Remember how an even number is a number that is divisible by 2?



**설명:**     
짝수는 `2`로 나누어지는 것을 기억하고 있는가?     
`2`로 나누어지는 숫자는 짝수이다. 짝수인지를 어떻게 알수 있는지 공부해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function **`is_even`** that will take a number **`x`** as input.

If **`x`** is even, then return **True**.

Otherwise, return **False**.


**설명:**     
① 함수 `is_even(x)`을 만들어라. `x`가 짝수이면 True를 반환하고, 홀수이면 False 를 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The modulo **`%`** operation is useful for determining if one number is divisible by another.

Make sure to return True instead of printing it!


**설명:**     
`%` 연산자는 하나의 숫자를 나누어서 남는 나머지를 반환해 주는 연산자이다. 나머지가 0인것은 나누어서 떨어진다는 의미이다. 즉 2로 나누어서 나머지가 0이면, 그것은 짝수인것이다. 단, 0은 제외이다. 함수를 만들고 해당 함수를 호출하고 출력하는것을 잊지 말라.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_even(x):
  if x % 2 == 0:
    return True
  else:
    return False
  
print is_even(5)
print is_even(6)
```

**설명:**     
`is_even(5)`를 호출하면 함수 `is_even()`이 호출되어 x가 2로 나누어 0으로 떨어지는지를 점검한다. 2로 떨어지면 True를 반환하고, 그렇지 않으면 False를 반환한다.
{: .notice--info}


**결과** 
``` 
False
True
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 3. is_int    

An integer is just a number without a decimal part (for instance, -17, 0, and 42 are all integers, but 98.6 is not).

For the purpose of this lesson, we'll also say that a number with a decimal part that is all 0s is also an integer, such as 7.0.

This means that, for this lesson, you can't just test the input to see if it's of type int.

If the difference between a number and that same number rounded is greater than zero, what does that say about that particular number?

 



**설명:**     
정수(integer)는 소수가 없는 10진수이다. (예, 소수점 있는 수 98.6), 그리고, 소수점 있는 수(예, 7.0)도 정수이다. 프로그램에서 정수인지를 어떻게 파악 할수 있을까? 우리는 어떤 수에서 그수를 반올림 한 값의 차리를 봐서, 0이면, 정수이고, 0이 아니면 정수가 아니라고 알수 있다.  이장에서 이것에 관하여 공부해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function **`is_int`** that takes a number **`x`** as an input.

Have it return True if the number is an **integer** (as defined above) and **False** otherwise.

For example:
```python
is_int(7.0)   # True    
is_int(7.5)   # False    
is_int(-1)    # True
```


**설명:**     
① 함수 `is_int(x)`를 만드시오. 이 함수는 입력값 `x`가 정수(interger)이면 True를 반환하고, 아니면 False를 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To use the function **`abs()`**, **`round()`**


**설명:**     
내장 함수 `abs()`는 절대값을 반환하고, `round()`는 소수점을 버린 정수만을 반환한다. 이를 활용하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_int(x):
  absolute = abs(x)
  rounded = round(absolute)
  return absolute - rounded == 0

print is_int(10)
print is_int(10.5)
```

**설명:**     
함수 `is_int(x)`는 입력값 `x`를 절대값을 구하고, 이 값에서 round한 값을 뺀다. 이 두 수의 차이가 0보다 크면 이 `x`값은 정수가 아니다.
{: .notice--info}



**결과** 
``` 
True
False
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 4. digit_sum    

Awesome! Now let's try something a little trickier. Try summing the digits of a number. 



**설명:**     
각 자리별 수를 더하여 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function called **`digit_sum`** that takes a **positive integer `n`** as input and returns the **sum of all** that number's digits. For example: digit_sum(1234) should return 10 which is 1 + 2 + 3 + 4. (Assume that the number you are given will always be positive.)

Check the hint if you need help!


**설명:**     
① 함수 `digit_sum(n)`을 만들어 보자. 이 함수는 입력된 `n`값의 각 자리 수를 더하여 결과를 반환하는 함수이다. 예를 들면 `digit_sum(1234)`이면 반환값은 10이다. 즉, 1+2+3+4=10 인 것이다. 입력값은 항상 양수만 들어가야 한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
One way might be to convert the integer to a string with **`str()`**, iterate over it, and turn the substrings back into integers with **`int()`** to do the addition.

If you're looking for a challenge, try this: to get the rightmost digit of a number, you can modulo **`(%)`** the number by 10. To remove the rightmost digit you can floor divide (//) the number by 10. (Don't worry if you're not familiar with floor division—you can look up the documentation here. Remember, this is a challenge!)

Try working this into a pattern to isolate all of the digits and add them to a total.




**설명:**     
`str()`함수를 사용하여 입력값을 문자열로 바꾼다. for 문을 돌면서 각 값을 빼내어 `int()`를 사용하여 변환한다. 각 값을 합한다. 그외에도 `%`연산자를 사용하여 10으로 나누어 나머지 값을 더하면 되는 방법도 있다. 한번 시도해 봐라. `%`와 비슷한 `//` 연산자도 있다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def digit_sum(n):
  total = 0
  string_n = str(n)
  for char in string_n:
    total += int(char)
  return total

#Alternate Solution:

#def digit_sum(n):
#  total = 0
#  while n > 0:
#    total += n % 10
#    n = n // 10
#  return total
  
print digit_sum(1234)
```

**설명:**     
입력값 `n`을 문자열로 바꾼다. 그리고 문자열을 하나씩 뽑아내서 `int(char)`숫자로 바꾼다. `total`변수에 각 값을 더한다.    
또다른 방법은 입력값 `n`을 `%10`을 하여 제일 마지막 자릿수 4를 반환하여 전체 `total`값에 더한다. `n`값을 `//10`하여 마지막 자릿수를 버리고 `123`을 다시 `%10`으로 나누어 나머지 3을 `total`변수에 저장한다.
{: .notice--info}



**결과** 
``` 
10
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 5. factorial    

All right! Now we're cooking. Let's try a **factorial problem**.

To calculate the factorial of a non-negative integer **x**, just multiply all the integers from **1 through x**. For example:

factorial(4) would equal 4 * 3 * 2 * 1, which is 24.
factorial(1) would equal 1.
factorial(3) would equal 3 * 2 * 1, which is 6.




**설명:**     
수학이 factorial(계승)을 구현해 보자. `factorial(3)`은 6 이다. 계산하는 방법은 3 x 2 x 1 = 6 이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function **`factorial`** that takes an integer **`x`** as input.

Calculate and return the factorial of that number.


**설명:**     
① 함수 `factorial(x)`를 만들어라. `factorial(x)` 함수는 입력한 값의 계산값을 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Consider having **`factorial()`** call itself. When the input is 1, your function could just return 1. Otherwise, it could return the number multiplied by **`factorial(n - 1)`**.

Note that mathematically, factorial(0) is 1.


**설명:**     
`facotorial(x)`함수는 `n` 값이 1이 될때까지 자신의 함수를 호출한다. 그리고 최종적으로 `factorial(0)`이면 값은 1을 반환한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def factorial(x):
    total = 1
    while x>0:
        total *= x
        x-=1
    return total
  
print factorial(5)

# def factorial2(n):
#     if n == 0:
#         return 1
#     else:
#         return n * factorial2(n-1)

# print factorial2(5)      
```

**설명:**     
`x`값을 1씩 줄여가면서 `total`값에 곱해 준다. `x`가 1이 될때까지 while문을 돌면서 진행한다.    
또다른 방법은 `factorial2(n-1)`을 하는 방법이다. 자신의 함수를 다시 호출해서 사용하는 방법으로 나중에 배우게 될 것이다. 
{: .notice--info}



**결과** 
``` 
120
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 6. is_prime    

A prime number is a positive integer greater than 1 that has no positive divisors other than 1 and itself. (That's a mouthful!)

In other words, if you want to test if a number in a variable **`x`** is prime, then no other number should go into **`x`** evenly besides 1 and x. So 2 and 5 and 11 are all prime, but 4 and 18 and 21 are not.

If there is a number between 1 and x that goes in evenly, then x is not prime.





**설명:**     
prime(소수)는 1 과 자신 이외에는 나눌수 없는 값을 말한다. 어떤 입력값 `x`를 입력해서 소수 인지를 확인하는 함수를 만들어 보자. 1, 2, 3, 5, 7, 11은 소수의 예이다. 4는 2로 나누어 지기에 소수가 아니다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`is_prime`** that takes a number **`x`** as input.

For each number n **from 2 to x - 1**, test if x is evenly divisible by **n**.

If it is, return False.

If none of them are, then return True.


**설명:**     
① 함수 `is_prime(x)`를 만들어라. 이 함수는 1과 자신 `x`이외에는 나누어 지지 않는다. 즉 2부터 `x-1`까지 값으로 나누어서 0이 나오면 소수가 아니기에 False를 반환하고, 그렇지 않으면 True를 반환하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember: all numbers less than 2 are not prime numbers!


**설명:**     
2보다 작은 모든 숫자는 소수가 아니다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def is_prime(x):
    if x < 2:
        return False
    else:
        for n in range(2, x-1):
            if x % n == 0:
                return False
        return True

print is_prime(13)
print is_prime(10)
```

**설명:**     
입력값 `x-1`값이 될때까지 2부터 나머지를 구해서 나누어지는 상황(`x%n==0`)이 발생하면 소수가 아니기에 False를 반환하고, 그외에는 True를 반환한다. 입력값이 2보다 작은 값이 들어오면 무조건 False를 반환한다. 
{: .notice--info}



**결과** 
``` 
True
False
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 7. reverse    

Great work so far! Let's practice writing some functions that work with strings.



**설명:**     
문자열을 조작하는 방법을 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`reverse`** that takes a string textand returns that string in reverse. For example: reverse("abcd") should return "dcba".

You may not use reversed or [::-1] to help you with this.

You may get a string containing special characters (for example, !, @, or #).


**설명:**     
① `reverse()`함수를 만들어 보자. 이 함수는 입력한 문자열을 반대로 출력해주는 함수이다. 예를 들면 `reverse("abcd")`를 입력하면 "dcba"를 반환해 준다.    
물론, 앞에서 배운 `[::-1]`, `reversed()`을 사용해도 되지만, 여기서는 직접 함수를 만들어 본다. 특수 문자도 포함된다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Consider how you would loop through text starting from the last character through the first character.


**설명:**     
입력받은 문자열의 마지막 부터 추출하여 리스트에 저장한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def reverse(text):
    word = ""
    l = len(text) - 1
    while l >= 0:
        word = word + text[l]
        l -= 1
    return word
  
print reverse("Hello World")
#print ''.join(reversed("abcd"))
#print ("Hello world")[::-1]

```

**설명:**     
입력한 문자열의 길이 -1 만큰 반복한다. 그리고 마지막 문자 index 값으로 읽어서 `word`에 저장한다. 
{: .notice--info}



**결과** 
``` 
dlroW olleH
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 8. anti_vowel    

Nice work. Next up: vowels!



**설명:**     
모음을 찾아서 조작하는 방법을 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`anti_vowel`** that takes one string, **`text`**, as input and returns the text with all of the **vowels removed**.

For example: anti_vowel("Hey You!") should return "Hy Y!". Don't count Y as a vowel. Make sure to remove lowercase and uppercase vowels. 


**설명:**     
① 함수 `anti_vowel(text)`을 만들어라. 이 함수는 모음을 찾아서 없앤 문자열을 반환한다. 예를 들면 `anti_vowel("Hey You!")`를 호출하면, "Hy Y!"를 반환한다. 단, 대문자 "Y"를 없애지 말라. 그 외 대/소문자 모음 모두를 삭제하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
To check to see if **`c`** is a vowel, you can do: c in "aeiouAEIOU".


**설명:**     
모음 모둠인 "aeiouAEIOU"에 해당 문자가 속하는지를 점검한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def anti_vowel(text):
    result = ""
    vowels = "ieaouIEAOU"
    for char in text:
          if char not in vowels:
            result += char
    return result

print anti_vowel("hello book")
```

**설명:**     
입력한 문자열을 한 글자씩 추출하여 "ieaouIEAOU"에 속하는지를 점검하여, 속하지 않으면 문자열을 저장하여 반환한다. 
{: .notice--info}



**결과** 
``` 
hll bk
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 9. scrabble_score    

Scrabble is a game where players get points by spelling words. Words are scored by adding together the point values of each individual letter (we'll leave out the double and triple letter and word scores for now).

To the right is a dictionary containing all of the letters in the alphabet with their corresponding Scrabble point values.

For example: the word "Helix" would score 15 points due to the sum of the letters: 4 + 1 + 1 + 1 + 8.

 



**설명:**     
Scrabble 게임은 각 알파벳에 다른 점수를 매겨서, 각 단어의 알파벳 점수를 합한 값을 가지는 게임이다. 우리는 기존에 배운 딕셔너리 변수에 각 알파벳의 점수를 할당하여 각 단어별 점수를 매긴다. 예를 들면, "Helix"는 각 알파벳 점수는 H:4, e:1, l:1, i:1, x:8이다 이들 점수의 합은 15점이다. Scrabble 게임을 통하여 딕셔너리 활용법을 배워보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function **`scrabble_score`** that takes a string **`word`** as input and returns the **equivalent scrabble score** for that word.

* Assume your input is only one word containing no spaces or punctuation.
* As mentioned, no need to worry about score multipliers!
* Your function should work even if the letters you get are uppercase, lowercase, or a mix.
* Assume that you're only given non-empty strings.


**설명:**     
① 함수 `scrabble_score(word)`를 만들고, 이 함수는 입력한 `word`의 점수를 반환한다.     
• 입력 단어는 공백이나, 구두점이 없어야 한다.     
• 점수 배열에 대해서는 걱정하지 마라.      
• 함수는 대문자, 소문자, 또는 대/소문자가 섞여 있어도 동작한다.     
• 입력은 반드시 해야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Have your function loop through the word that you are given as input and look up the score for each letter in the score dictionary. Add the score for each letter into a total of some sort.

Remember you can use a string's .lower() method to make your string lower case!




**설명:**     
입력된 워드의 알파벳을 순차적으로 `score` 딕셔너리에 있는 각 알파벳 점수를 참조하여 더한다.    
모든 입력된 문자는 `.lower()`를 사용하여 소문자로 일원화 하여 `score`딕셔너리에서 찾는다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
score = {"a": 1, "c": 3, "b": 3, "e": 1, "d": 2, "g": 2, 
         "f": 4, "i": 1, "h": 4, "k": 5, "j": 8, "m": 3, 
         "l": 1, "o": 1, "n": 1, "q": 10, "p": 3, "s": 1, 
         "r": 1, "u": 1, "t": 1, "w": 4, "v": 4, "y": 4, 
         "x": 8, "z": 10}
         
def scrabble_score(word):
  word = word.lower()
  total = 0
  for letter in word:
    for leter in score:
      if letter == leter:
        total = total + score[leter]
  return total

print scrabble_score("pizza")

# def scrabble_score(word):
#   totla = 0
#   for i in word:
#      w = i.lower()
#      r = score[w]
#      totla += r
#   return totla

# print scrabble_score("pizza")
```

**설명:**    
입력 문자열 `word.lower()`로 소문자로 일원화한다.    
전체값을 저장할 변수 `total`을 초기화 한다.    
변수 `word`의 글자를 하나씩 뽑아낸다.    
그 뽑아낸 글자를 딕셔너리 `score`에서 반복적으로 찾는다.    
찾았으면, 그 글자가 맞는지 다시한번 확인하고.   
변수 `total`에 해당 글자의 점수를 더한다.     
결과를 반환한다. 
{: .notice--info}




**결과** 
``` 
25
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 10. censor    

You're doing great with these string function challenges. Last one!



**설명:**     
문자열 조작 기능을 하나더 연습해 봅시다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Write a function called **`censor`** that takes two strings, **`text`** and **`word`**, as input. It should return the text with the word you chose **replaced with asterisks**. For example:
```python
censor("this hack is wack hack", "hack")
```
should return:
```python
"this **** is wack ****"
```
* Assume your input strings won't contain punctuation or upper case letters.
* The number of asterisks you put should correspond to the number of letters in the censored word.



**설명:**     
① 함수 `censor(text, word)`를 만들어라. 이 함수는 입력받은 `text`중 `word`글자 부분만 `*`로 변경하는 함수이다.     
• 대문자는 사용하지 않는다
• `*`로 대체할때, `word` 수 만큼만 `*`로 대체해야 한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use
```python
string.split()
# and 
" ".join(list)
```
to help you here.

Remember: "*" * 4 equals "****"

After splitting the string with string.split(), you can loop through the indices in the list and replace the words you are looking for with their asterisk equivalent. Join the list at the end to get your sentence!




**설명:**     
`string.split()`와 `" ".join(list)`를 활용 할수 있다.    
`"*" * 4 -> "****"`이 만들어 진다.    
입력된 문자열의 분리하여, 반복하며 돌면서 해당 문자가 대치할 문자와 같은지를 비교하여 찾아 낸다.     
해당 문자를 찾았으면 그 문자 크기만큼 "*"를 변경하고, 해당 문자열을 리스트에 저장한다.    
마지막에 저장된 리스트를 하나의 스트링으로 만든다.그리고 반환한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def censor(text, word):
    words = text.split()
    result = ''
    stars = '*' * len(word)
    count = 0
    for i in words:
        if i == word:
            words[count] = stars
        count += 1
    result =' '.join(words)

    return result
  
print censor("this hack is wack hack", "hack")


# def censor2(text, word):
#   low_text = text.lower()
#   low_word = word.lower()
  
#   list_text = []
#   for t in low_text.split():
#     if t == low_word:
#        t = "*" * len(t)
#        list_text.append(t)
#     else:
#       list_text.append(t)
  
#   return " ".join(list_text)

# print censor2("this hack is wack hack", "hack")
```

**설명:**     
입력 받은 문장을 잘라서 리스트 `words`에 넣는다.    
결과물을 저장할 변수 `result`를 초기화한다.    
`*`로 변경할 `word` 갯수를 계산하여 변수 `star`에 저장한다. 
리스트 `words`에서 하나씩 꺼내어, 변경할 `word`와 같은 지 확인한다.    
리스트 `words`의 변경할 인덱스`words[count]`에 `star`를 저장한다.    
리스트 `words`를 문자열로 변경하여 반환한다. 
{: .notice--info}



**결과** 
``` 
this **** is wack ****
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 11. count     

Great work so far. Let's finish up by practicing with a few functions that take lists as arguments.



**설명:**     
리스트를 arguments로 가지는 함수들에 대해서 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`count`** that has two arguments called **`sequence`** and **`item`**.

Return the number of times the item occurs in the list.

For example: count([1, 2, 1, 1], 1) should return 3 (because 1 appears 3 times in the list).

* There is a list method in Python that you can use for this, but you should do it the long way for practice.
* Your function should return an integer.
* The item you input may be an integer, string, float, or even another list!
* Be careful not to use list as a variable name in your code—it's a reserved word in Python!



**설명:**     
① 함수 `count(sequence, item)`을 만들어라.
예를 들면 `count([1,2,1,1], 1)`을 호출하면 3이 반환된다. 이유는 1이 리스트에 3개가 들어 있기 때문이다.    
• python 자체 내장 함수에서 리스트의 특정 항목의 갯수를 찾아주는 기능이 있지만, 연습을 위해서 우리는 직접 만들어 보자    
• return(반환값)은 정수(integer) 이다.    
• 입력값은 정수(integer), 문자(string), 실수(float) 또는 다른 것일 수 있다.    
• 리스트 변수명을 정할때, python에서 예약된 코드(ex, if )를 사용하면 안된다.    
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can set a **`sum`** variable inside count. You can then iterate over sequence and increment **`sum`** every time you find an element in the sequence that matches item.


**설명:**     
변수 `sum`을 만들어, 찾고자 하는 숫자와 같은 것이 있으면 `sum`을 1씩 증가시킨다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def count(sequence, item):
    count = 0
    for i in sequence:
        if i == item:
            count += 1
    return count
  
print count([1, 2, 1, 1], 1)
```

**설명:**     
리스트 [1,2,1,1]을 입력받고, 이중 1이 몇개 있는가를 찾는 프로그램이다.    
`sequence=[1,2,1,1]`에서 `i`가 하나씩 추출하여, `if i==item`비교하여 일치하면, 변수 `count`를 1씩 증가시킨다. for 문이 끝나고 최종 `count`값을 return(반환)한다.
{: .notice--info}



**결과** 
``` 
3
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 12. purify    

Awesome! Now let's practice filtering a list. 



**설명:**     
리스트의 필터링을 연습해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`purify`** that takes in a list of numbers, **removes all odd numbers** in the list, and **returns the result**. For example, purify([1,2,3]) should return [2].

**Do not directly modify** the list you are given as input; instead, return a new list with only the **even numbers**.




**설명:**     
① 함수 `purify(list)`를 만들어라. 이 함수는 리스트의 값중 홀수를 삭제하고 해당 리스트를 return(반환) 하는 함수이다.     
• 입력받은 리스트를 바로 수정하지 말고, 새로운 리스트를 만들어 결과값을 저장하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Your code should share something in common with the **`is_even`** function you defined earlier.


**설명:**     
앞에서 연습한 함수 `is_even()`의 기능을 활용하여 홀수인지 짝수인지를 판단하라.     
`if i % 2 == 0` 이면 짝수이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def purify(lst):
    res = []
    for ele in lst:
        if ele % 2 == 0:
            res.append(ele)
    return res
  
print purify([1, 2, 3, 4])
```

**설명:**     
리스트 `lst`를 입력받고, 새로운 빈 리스트 `res`를 초기화 하자.     
`lst`의 값을 추출하여 `ele` 변수에 저장하고, 이 `ele`변수가 짝수인지를 (`ele % 2==0`)를 검사하여 짝수이면 리스트 `res=[]`에 추가한다. for 반복문이 끝나면 그 결과값을 return(반환)한다.
{: .notice--info}



**결과** 
``` 
[2, 4]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 13. product    

Great! Now let's try a little multiplication.



**설명:**     
리스트의 내용을 곱해 보자.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Define a function called **`product`** that takes a list of integers as input and **returns** the product of all of the elements in the **list**. For example: product([4, 5, 5]) should return 100 (because 4 * 5 * 5 is 100).

Don't worry about the list being empty.
Your function should return an integer.



**설명:**     
① 함수 `product(lst)`를 만들어 보자. 이 함수는 정수를 입력값으로 가지면 리스트의 모든 값을 곱한 결과를 return(반환)한다. 예를 들면 `product([4,5,5])`를 호출하면, return(반환)값은 100 이다.    
• 리스트가 비어 있을 경우는 없다.    
• return(반환)값은 정수이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
You can use a loop to go through the elements of the list.

It'll probably be useful to use the **`*=`** operator.

Be careful **not to start your total at 0**, as this would make the overall result of the multiplication equal to 0! (Anything multiplied by zero equals zero.)




**설명:**     
입력받은 리스트의 값을 하나씩 추출하여 `*=` 기능을 사용하여라.    
전체 값을 담는 변수 `total`의 초기값은 0으로 해선 안된다. 이유는 곱셈에서 0은 어떤 값을 곱해도 0이다. `total` 초기값은 1로 초기화하라.  
{: .notice--info}

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
def product(list):
  total = 1
  for num in list:
    total = total * num
    #total *=num
  return total

print product([4, 5, 5])
```

**설명:**     
입력받은 리스트 `list`의 항목 값을 하나씩 추출하여 변수 `total`값에 곱한다. 최종적으로 `total`값을 return(반환)한다. 
{: .notice--info}


**결과** 
``` 
100
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 14. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

**결과** ``` ```

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```



<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 15.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 16. 



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 17.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 18.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PRACTICE MAKES PERFECT</font> 
### 19.



**설명:** 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** 


**설명:** ① 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    



**설명:** 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
```

**설명:** 
{: .notice--info}


**결과** ``` ```


<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
