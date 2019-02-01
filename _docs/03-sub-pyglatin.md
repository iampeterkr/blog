---
# layout : rchive
title: "PygLatin"
permalink: /pyglatin/
excerpt: "We exercise until learning Python Syntaxk"
last_modified_at: 2018-11-30T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---

<hr style="border: solid 1px #dddddd ;">    

LESSON    

In this lesson we'll put together all of the Python skills we've learned so far including string manipulation and branching. We'll be building a Pyg Latin translator. (That's Pig Latin for Python Programmers!)    


**설명:** [ 학습방향 ]     
이 장에서는 지금까지 배운 것을 복습 해보자. 
{: .notice--info}     
     

    
    
    
<hr style="border: solid 1px #dddddd ;">


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 
### 1.  Break It Down    

Now let's take what we've learned so far and write a Pig Latin translator.

Pig Latin is a language game, where you move the first letter of the word to the end and add "ay." So "Python" becomes "ythonpay." To write a Pig Latin translator in Python, here are the steps we'll need to take:

1. Ask the user to input a word in English.
2. Make sure the user entered a valid word.
3. Convert the word from English to Pig Latin.
4. Display the translation result.



**설명:** [ Learn ]    
• 지금까지 배운 Python 문법을 정리할 겸 배운것을 활용하여 응용 프로그램을 만든다.    
• 1st : 단어를 입력받아라.    
• 2nd : 입력 받은 단어를 비교하고 체크하라.    
• 3rd : 입력 받은 단어를 Pig Latin 문자로 변경하라.    
• 4th : 그 결과를 출력하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* When you're ready to get coding, click `Next`. Since we took the time to write out the steps for our solution, you'll know what's coming!


**설명:** [ Instruction ]    
• Coding 창의 소스가 이해가 되면, 마음의 준비가 되었으면, Next 를 클릭하라. 
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
* skip

```python
skip
```

**설명:** [ Solution ]    
• skip
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
<font size="3"  face="돋움">PYGLATIN</font> 

### 2. Ahoy! (or Should I Say Ahoyay!)    

Let's warm up by **printing** a welcome message for our translator users.


**설명:** [ Learn ]    
• 몸 풀기로  print 를 해보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Please **print** the phrase "Pig Latin".


**설명:** [ Instruction ]    
• 'print "Pig Latin' 을 실행하라.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

```python
print " Hellow World"
```
**설명:** [ Hint ]    
• print " Hellow World" 라고 사용한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
print "Pig Latin"
```

**설명:** [ Solution ]    
• print 문을 사용하여 문자 "Pig Latin"을 출력한다. 
{: .notice--info}


**결과** 
```
Pig Latin
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 3.  Input!    

Next, we need to ask the user for input.    

```python
name = raw_input("What's your name?")
print name
```    

In the above example, `raw_input()` accepts a string, prints it, and then waits for the user to type something and press Enter (or Return).

In the interpreter, Python will ask:

```
What's your name?
```    

Once you type in your name and hit Enter, it will be stored in name.


**설명:** [ Learn ]     
• Console 창에 다음과 같은 문자열이 출력된다.    
• "What's your name?"     
• Console 창에 당신의 이름을 입력하라. 그리고 Enter를 클릭하라.        
• # 함수 raw_input() 는 console 창에 문자열을 입력받는 함수이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)

* On line 4, use **raw_input("Enter a word: ")** to ask the user to enter a word. Save the results of `raw_input()` in a variable called original.

* Click `Run`

* Type a word in the console window and press Enter (or Return).



**설명:** [ Instruction ]    
• 함수 raw_input() 를 사용하여 다음과 같이 Editor 창에 코딩하라.    
• ' raw_input("Enter a word: ") '
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Your code should look something like this:   

```python
variable_name = raw_input('Prompt')
```    

* Does it look like your code is stuck?     
* Is there a spinning circle?     
* That probably means that your code is waiting for you to type something!     
* Click inside the console window on the other side, type a word, then press Enter (or Return).



**설명:** [ Hint ]    
• 함수 raw_input() 은 Console 창에서 문자열을 입력 받는 함수이다.    
• 'Prompt'는 console 창에 출력되는 질문 메시지 이다.     
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print 'Welcome to the Pig Latin Translator!'

# Start coding here!
original = raw_input("Enter a word:")
```

**설명:** [ Solution ]    
• 함수 ' raw_input("Enter a word:") ' 로 문자를 입력 받는다.
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
<font size="3"  face="돋움">PYGLATIN</font> 

### 4. Check Yourself!    

Next we need to ensure that the user actually typed something.

```python
empty_string = ""
if len(empty_string) > 0:
  # Run this block.
  # Maybe print something?
else:
  # That string must have been empty.
```  

We can check that the user's string actually has characters!


**설명:** [ Learn ]    
• 변수 empty_string 를 빈 문자열로 초기화 한다.    
• 변수 empty_string 에 저장된 문자열의 길이를 함수 len() 을 사용하여 구한다.    
• 변수 empty_string 의 길이가 0보다 큰지를 비교한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Write an `if` statement that verifies that the string has characters.

* Add an `if` statement that checks that `len(original)` is greater than zero. Don't forget the : at the end of the if statement!    

* If the string actually has some characters in it, **print** the user's word.

* Otherwise (i.e. an `else`: statement), please print **"empty"**.

* You'll want to run your code multiple times, testing an empty string and a string with characters. When you're confident your code works, continue to the next exercise.


**설명:** [ Instruction ]    
• if 문을 사용하여 입력 받은 값이 문자열인지 확인한다.    
• if 문의 조건절에서 변수 original 의 길이를 len() 함수를 이용하여 구한다.    
• if 문의 조건절에서 len(original) 값이 0 보다 큰지 비교한다.     
• # if 문 끝에는 ( : ) 을 꼭 확인한다.     
• else 문에서는 변수 original 에 문자가 입력되지 않으면, empty 를 출력한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* Don't forget that `>` is the greater than operator!

* Does it look like your code is stuck? Is there a spinning circle?    
* That probably means that your code is waiting for you to type something!    
* Click inside the console window on the other side, type a word, then press Enter (or Return).


**설명:** [ Hint ]    
• 같거나 크다 :  >=    
• 크다      :  >     
• # Console 에서 문자를 입력하고 Enter 를 클릭하면 입력이 되는 것이다  
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
print 'Welcome to the Pig Latin Translator!'

# Start coding here!
original = raw_input("Enter a word:")
if len(original) > 0:
  print original
else:
  print "empty"
```

**설명:** [ Solution ]    
• 변수 original 에 Console 에서 입력값 이 들어가 있다.    
• 변수 original 에 문자가 들어가 있으면 해당 문자를 출력한다.(if 문)    
• 변수 original 에 문자가 없으면 "empty"를 출력한다.(else 문). 
{: .notice--info}



**결과** 
```
# Input the string, hellow, and Click the `Enter`
Welcome to the Pig Latin Translator!
Enter a word:hellow
hellow

# No input and Click the `Enter`
Welcome to the Pig Latin Translator!
Enter a word:
empty
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 5. Check Yourself... Some More    

Now we know we have a non-empty string. Let's be even more thorough and check that our string only contains letters.

Consider the following code:

```python
x = "J123"
x.isalpha()  # This will return 'False'
```

In the first line, we create a string with letters and numbers.

The second line then runs the method `.isalpha()` which returns False since the string contains non-letter characters.

You can use `.isalpha()` to check that a string doesn't contain any non-letter characters! For example:


**설명:** [ Learn ]    
• 함수 .isalpha() 은 변수 x 에 저장된 값이 알파벳 인지 검증한다.    
• 변수 x 에 알파벳이 있으면 True 값을 반환한다.    
• 변수 x 에 알파벳이 없으면 False 값을 반환한다.  
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Use and to add a second condition to your `if` statement.     
* In addition to your existing check that the string contains characters, you should also use `.isalpha()` to make sure that it only contains letters.

* Don't forget to keep the **colon** at the end of the `if` statement!


**설명:** [ Instruction ]     
• 함수 .isalpha() 를 사용하여 변수에 입력된 값에 알파벳 포함 여부를 획인하라.    
• # 주의 : if 조건문 맨끝에 ( : ) 쓰는 것을 주의하자.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
* To combine multiple conditions in one `if`, you can use and between the two conditions, like this:

```python
if has_chars(the_string) and the_string.isalpha():
  print the_string
else:
  print "empty"
```

**설명:** [ Hint ]    
• if 문의 조건절에는 1 개 이상의 조건들이 들어갈 수 있다.     
• ' the_string.isalpha() ' 은 변수 the_string 에 알파벳이 있는지 점검한다.
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    

```python
print 'Welcome to the Pig Latin Translator!'

# Start coding here!
original = raw_input("Enter a word:")
if len(original) > 0 and original.isalpha():
  print original
else:
  print "empty"
```

**설명:** [ Solution ]     
• if 문에서는 2가지를 비교한다.    
• 1st : 변수 original 에 값이 들어 있는지 ( if len(origial) > 0)    
• 2nd : 변수 original 에 알파벳이 들어 있는지 ( original.isalpha() )    
• 그 외( else )에는 "empty"를 출력한다.
{: .notice--info}



**결과** 
```
# Input the string "Hellow"
Welcome to the Pig Latin Translator!
Enter a word:Hellow
Hellow
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 6. Pop Quiz!    

When you finish one part of your program, it's important to test it multiple times, using a variety of inputs. 



**설명:** [ Learn ]    
• 프로그램을 만들었으면 다양하게 입력하면서 테스트 해 보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Take some time to **test your current code**.     
* Try some inputs that should pass and some that should fail.     
* Enter some strings that contain **non-alphabetical** characters and an **empty** string.

* When you're convinced your code is ready to go, click Next to move forward!


**설명:** [ Instruction ]    
• 현재 코드를 이용하여 테스트를 하라.    
• 통과할 값(알파벳이 포함된)과 실패할 값(알파벳이 없을 값)을 넣어라.    
• 알파벳이 포함된 문자열도 넣고, 없는것도 넣어라.    
• 소스가 확실히 이해가고, 다음 장으로 넘어갈 준비가 되면 다음장으로 넘어가라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* No trick here! Just test your code to make sure it works as expected.

**설명:** [ Hint ]    
• 특별한 것이 없다. 그냥 테스트 하면 된다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
print 'Welcome to the Pig Latin Translator!'

# Start coding here!
original = raw_input("Enter a word:")
if len(original) > 0 and original.isalpha():
  print original
else:
  print "empty"
```

**설명:** [ Solution ]    
• 변수 original 에 입력된 문자열이 존재하고 알파벳이면 포함되어 있는지 비교한다.    
• if 조건절을 만족하면 변수 original 값이 출력된다.    
• 그렇지 않으면 "empty" 가 출력된다. 
{: .notice--info}



**결과** 
``` 
Welcome to the Pig Latin Translator!
Enter a word:abc_d
empty
```

```
Welcome to the Pig Latin Translator!
Enter a word:abcd
abcd
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 7. Ay B C    

Now we can get ready to start translating to Pig Latin! Let's review the rules for translation:

You move the first letter of the word to the end and then append the suffix 'ay'. Example: python -> ythonpay

Let's create a variable to hold our translation suffix.


**설명:** [ Learn ]    
• 이 장에서는 문자열을 제어하는 방법을 배워보자.    
• "python" 의 첫글지 "p" 를 "python" 의 제일 뒤로 보낸다.        
• 그다음에 문자열 "ay" 를 붙이자.    
• e.g. "python" -> "ythonpay"    
• 문자 "ay" 를 담을 변수를 만든다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

* Create a variable named `pyg` and set it equal to the suffix 'ay'.


**설명:** [ Instruction ]    
• 변수 pyg 를 만들고 여기에  문자열 'ay' 를 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

* Remember to use a single equal sign to do the assignment and to put quotation marks around the string **'ay'**!

**설명:** [ Hint ]    
• 문자열을 변수에 대입 할때는 (' ')를 사용한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
pyg = 'ay'
```

**설명:** [ Solution ]    
• 변수 pyg 를 생성하고 문자열 'ay' 를 입력한다. 
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
<font size="3"  face="돋움">PYGLATIN</font> 

### 8. Word Up
Let's simplify things by making the letters in our word **lowercase**.

```python
the_string = "Hello"
the_string = the_string.lower()
```
The `.lower()` function does not modify the string itself, it simply returns a lowercase-version. In the example above, we store the result back into the same variable.


**설명:** `.lower()`함수 기능은 단순히 문자열을 변경하는 것이 아니라, 단순히 소문자로 변경하는 것이다. 변수 `the_string`에 저장된 문자열을 다시 소문자로 변경하여 다시 변수 `the_string`에 저장한다.  
{: .notice--info}


We also need to grab the first letter of the word.

```python
first_letter  = the_string[0]
second_letter = the_string[1]
third_letter  = the_string[2]
```
Remember that we start counting from **zero**, not one, so we access the first letter by asking for **[0]**.

**설명:** 우리는 변수 `the_string`에 들어 있는 문자열의 개별 알파벳 문자를 추출할수 있다. 우리는 `index`주소를 0번 부터 시작한다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Inside your `if` statement:

• Create a new variable called word that holds the .lower()-case conversion of original.
• Create a new variable called first that holds word[0], the first letter of word.


**설명:** ① `if` 조건문에서, 변수 `word`를 만들고 해당 변수에 변수 `origanl`값을 소문자로 변경하여 대압히라.    
② 변수 `first`를 만들고 변수 `word[0]`주소의 값을 대입하라. `word[0]`은 첫번째 문자이다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

Use a variable called word to store the result of original.lower().

Use a variable called first to store the result of word[0].

And make sure that you do this inside your if statement.

Note: You can print out the values of the variables word and first to double-check your work (remove these print statements when you're done debugging).

Remember that the first letter of a string can be found at index 0, like this:

```python
first = "python"[0]
first # "p"
```


**설명:** 변수 `word`를 만들고, 해당 변수에 입력값을 소문자로 변경하여 저장하라. 그리고 변수 `word`의 첫번째 글자를 출력하라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
pyg = 'ay'

original = raw_input('Enter a word:')

if len(original) > 0 and original.isalpha():
  word = original.lower()
  first = word[0]
else:
    print 'empty'
```

**설명:** ① 입력변수 `original`의 소문자를 변수 `word`에 대입하고, ② `word`의 첫번째 글자 `word[0]`를 변수 `first`에 대입하라. 
{: .notice--info}



**결과** 
``` 
Enter a word:ABCD

```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 9. Move it on Back
Now that we have the first letter stored, we need to add both the letter and the string stored in pyg to the end of the original string.

Remember how to **concatenate** (i.e. add) strings together?

```python
greeting = "Hello "
name = "D. Y."
welcome = greeting + name
```

**설명:** 각각의 변수에 저장된 문자열을 `+`을 이용하여 문자열을 연결할 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** On a new line after where you created the `first` variable:

Create a new variable called `new_word` and set it equal to the concatenation of `word`, `first`, and `pyg`.


**설명:** ① 변수 `first`다음 라인에 변수 `new_word`를 만들고, ②`new_word`에 변수 `word`, `first`, `pyg` 문자열을 연결하여 대입하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

You can use `+` to concatenate (put together) two strings, like this:

```python
word + first + pyg
```

**설명:** `+`를 연결하여 문자열을 연결한다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
pyg = 'ay'

original = raw_input('Enter a word:')

if len(original) > 0 and original.isalpha():
  word = original.lower()
  first = word[0]
  new_word = word + first + pyg
else:
    print 'empty'
```

**설명:** 변수 `new_word`에 변수 `word`, `first`, `pyg`를 `+`를 사용하여 문자열을 연결한다.
{: .notice--info}



**결과** 
``` 
Enter a word:ABCD
# no display result
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 10. Ending Up
Well done! However, now we have the first letter showing up both at the beginning and near the end.

```python
s = "Charlie"

print s[0]
# will print "C"

print s[1:4]
# will print "har"
```
1. First we create a variable `s` and give it the string **"Charlie"**
2. Next we access the **first letter** of **"Charlie"** using `s[0]`. Remember letter positions start at **0**.
3. Then we access a slice of **"Charlie"** using `s[1:4]`. This returns everything from the letter at position `1` up till position `4`.
We are going to **slice** the string just like in the 3rd example above.


**설명:** ① 변수 `s`를 만들고 문자열 **"Charlie"**를 대입하고, ② 변수 `s[0]`는 첫번째 글자를 가리킨다. ③ 변수 `s`의 문자열을 다음과 같이 주면 `s[1:4]` 문자열 **"harl"**만 잘라낸다. 우리는 이번장에서는 문자열을 잘라내는 것을 연습한다.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Set `new_word` equal to the slice from the 1st index all the way to the end of `new_word`. Use [1:len(new_word)] to do this.


**설명:** ① 변수 `new_word`에 index 1번 문자열부터 변수 `new_word`에 들어있는 문자 끝까지를 잘내라. `[1:len(new_word)]`를 사용하라.
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

The first character in a string is at index `0`.

Remember that slicing a string looks a lot like accessing a single character.

```python
# single character
s[3]

# slice from 3 up until 6
s[3:6]
```
Advanced Tip! When slicing until the end of the string, instead of providing `len(new_word)`, you can also not supply the second index:

```python
my_string = "Python"
my_string[1:] # "ython"
```

**설명:** 문자열의 주소는 `0`부터 시작한다. `s[3]`은 실지로 4번째 문자열을 가리킨다. `s[3:6]`은 
`s[3]`부터 `s[6]`까지 문자열을 잘라낸다. `my_string[1:]`은 해당 변수 주소 1번부터 끝까지를 잘라낸다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
pyg = 'ay'

original = raw_input('Enter a word:')

if len(original) > 0 and original.isalpha():
  word = original.lower()
  first = word[0]
  new_word = word + first + pyg
  new_word = new_word[1:len(new_word)]
else:
    print 'empty'
```

**설명:** `new_word[1:len(new_word)]`는 변수 `new_word` 1번 주소 부터 변수 `new_word`에 저장되어 있는 문자열의 길이만큼 잘라내는 것이다. 
{: .notice--info}



**결과** 
``` 
Enter a word:ABCD
# no display result
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">PYGLATIN</font> 

### 11. Testing, Testing, is This Thing On?
Yay! You should have a fully functioning Pig Latin translator. Test your code thorougly to be sure everything is working smoothly.

You'll also want to take out any `print` statements you were using to help debug intermediate steps of your code. Now might be a good time to add some comments too! Making sure your code is clean, commented, and fully functional is just as important as writing it in the first place.


**설명:** 지금까지 작성한 프로그램을 테스트 해보자. 프로그래밍 사이에 `print`를 사용하여 해당 변수를 출력해보면서, 단계별로 어떻게 진행되었는지도 확인해 보자. 이해가 되었다면, 프로그램에 `#`를 사용하여 주석도 달아보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** When you're sure your translator is working just the way you want it, click Run Code to finish this project.


**설명:** ① 실행하여 테스트 해보자. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    

#skip

**설명:** `#skip`
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
pyg = 'ay'

original = raw_input('Enter a word:')

if len(original) > 0 and original.isalpha():
  word = original.lower()
  first = word[0]
  print first
  new_word = word + first + pyg
  print new_word
  new_word = new_word[1:len(new_word)]
  print new_word
else:
    print 'empty'
```

**설명:** ① 변수 `first`에는 `a`가 저장된다. ② 변수 `new_word`에는 `abcdefaay`가 저장된다. ③변수 `new_word`에 index 1번 문자부터 `new_word` 전체 길이 9번째 index 만큼 잘라낸다. 
{: .notice--info}



**결과** 
``` 
Enter a word:ABCDEF
a
abcdefaay
bcdefaay
```

<br>
<br>    
<br>    