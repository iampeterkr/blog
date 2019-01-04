---
# layout : rchive
title: "Battleship!"
permalink: /battleship/
excerpt: "Let's practice what we have learned so far."
last_modified_at: 2019-01-03T09:00:00-04:00
redirect_from:
  - /theme-setup/
toc: true
---
    
    
 <hr style="border: solid 1px #dddddd ;">

![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 1. Welcome to Battleship!    

In this project you will **build a simplified**, **one-player version of the classic board game Battleship**! In this version of the game, there will be a single ship hidden in a random location on a 5x5 grid. The player will have 10 guesses to try to sink the ship.

To build this game we will use our knowledge of lists, conditionals and functions in Python. When you're ready to get started, click Next to continue.

 



**설명:**     
지금가지 배운것을 활용하여 1인용 게임 'Battleship1'을 만들 것이다.  이 게임은 10번의 질문을 통하여 5x5 좌표 위에 숨어 있는 배의 위치를 찾아서 침돌 시키는 것이다. 이 게임은 우리가 이미 배운 리스트와 함수를 사용하여 개발 하것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Click Next to get started with Battleship!


**설명:**     
① Run을 실행하고 Next를 눌러 시작하자.  
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 2. Getting Our Feet Wet    

The first thing we need to do is to set up the game board. 



**설명:**     
우리가 첫번째로 해야 할일은 게임 판을 만드는 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a variable **`board`** and set it equal to an empty list.


**설명:**     
①  리스트 **`board`**를 만들고, 빈 리스트로 초기화 해라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
```python
lst=[]
```


**설명:**     
`lst=[]`은 변수 lst를 리스트로 초기화 하는 것이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
```

**설명:**     
변수 **`board = []`**를 빈 리스트로 초기화 하였다. 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 3. Make a List    

Good! Now we'll use a built-in Python function to generate our board, which we'll make into a **5 x 5** grid of **all "O"s, for "ocean."**
```python
print ["O"] * 5
```
will print out **['O', 'O', 'O', 'O', 'O']**, which is the basis for a row of our board.

We'll do this five times to make five rows. (Since we have to do this five times, it sounds like a loop might be in order.)





**설명:**     
바다에 "o"으로 채워진 5x5 판이 있다.  출력 해보면, 가로가 ["o", "o", "o", "o", "o"]인 판인 것이다. 우리는 이런 모양의 세로로 5개가 있는것을 만들 것이다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Create a 5 x 5 grid initialized to all **'O's** and store it in board.

* Use **`range()`** to **loop 5 times**.
* Inside the loop, **`.append()`** a list **containing 5 "O"s** to board, just like in the example above.
* Note that these are capital letter **"O"** and **not zeros**.




**설명:**     
① 5 x 5 판에 "O"로 채워진 변수 리스트 **`board`**를 만들어라.     

• **`range()`** 활용하여 5번 loop 반복해라.     
•  loop 안에서는 **`.append()`**를 이용하여 리스트 변수 **`board`**에 ["O","O","O","O","O"]가 5개가 있는 싱글 리스트를 만들어라. 
• 주의 할것은 "O"는 숫자가 아닌 영문 대문자 "O" 이다.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
What if you use a for loop that does the appending in the **`range (0,5)`**?

```python
[
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O']
]
```



**설명:**     
**`range(0,5)`**와 for 문을 활용하여 위 모양과 같은 리스트를 만들어라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
for i in range(5):
  board.append(['O'] * 5)
  
  
#print board
```

**설명:**     
**`['O'] * 5`**는 ['O','O','O','O','O']를 만드는 방법이다. 이를 for문으로 5번 loop를 돌려서 
`[
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O'],
  ['O','O','O','O','O']
]`를 만든다. 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 4. Check it Twice    

Great job! Now that we've built our board, let's show it off.

Throughout our game, we'll want to print the game board so that the player can see which locations they have already guessed. Regularly printing the board will also help us debug our program.

The easiest way to print the board would be to have Python display it for us using the print command. Let's give that a try and see what the results look like—is this a useful way to print our board for Battleship?





**설명:**     
print문을 통하여 **`board`** 리스트의 상태가 어떤지를 알 수 있다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** Use the print command to display the contents of the **`board`** list.


**설명:**     
① 리스트 **`board`**의 상태를 출력해 보자.   
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
The syntax for printing a list is 
```python
print list_name.
```

**설명:**     
리스를 출력하는 방법이다. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []
for i in range(5):
  board.append(['O'] * 5)
  
  
print board
```

**설명:**     
실행시켜 리스트 **`board`**가 어떤 상태인지를 확인한다. 
{: .notice--info}



**결과** 
``` 
[['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O'], ['O', 'O', 'O', 'O', 'O']]
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 5. Custom Print    

Now we can see the contents of our list, but clearly it would be easier to play the game if we could print the board out like a grid with each row on its own line.

We can use the fact that our board is a list of lists to help us do this. Let's set up a for loop to go through each of the elements in the outer list (each of which is a row of our board) and print them.



**설명:**     
리스트의 내용을 볼수 있지만, 더 편하게 볼수 있도록 고쳐 보자. 한줄에 좌~악 하고 나오는게 아니라, 5 X 5 모양으로 한줄씩 총 5줄이 보이는 형태로 고쳐 보다. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-instruction-01.png)    

**①** First, delete your existing **`print`** statement.

* Then, define a function named **`print_board`** with a single argument, **`board_in`**.

* Inside the function, write a for loop to iterates through each row in board and print it to the screen.

* Call your function with board to make sure it works.



**설명:**     
① 먼저, print 문을 삭제 하라.    
* 6라인에서 함수 **`print_board(board_in)`** 작성하여라.  
* 내부 기능으로, for 루프를 돌면선, 입력받은  **`board`** 의 값들을 `row`로 끄집어내라. 그리고 `row`를 출력하라.    
* 함수**`print_board(board)`**를 호출하여 잘 돌아 가는 확인하라. 
{: .notice--info}


<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-hint-01.png)    
Remember that the syntax to declare a function is **`def fun_name(parameters):`**. The syntax for iterating through a list is **`for x in list_name:`**


**설명:**    
함수는 `def fun_name(parameters):`로 사용해야 하면, for문은 `for x in list_name:`으로 사용해야 한다. 
for 문 다음에 def 문을 정의해라. 
{: .notice--info}

<br>
<hr/>


![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-solution-03.png)    


```python
board = []

for i in range(5):
  board.append(["O"] * 5)

def print_board(board_in):
  for row in board:
    print row
    
print_board(board)
```

**설명:**     
**`board`**에 `['O','O','O','O','O']`를 저장하고,    
**`print_board`** 함수를 만든다.     
**`print_board(board)`**를 호출한다.  
{: .notice--info}



**결과** 
``` 
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
['O', 'O', 'O', 'O', 'O']
```

<br>
<br>    
<br>    
![codecademy]({{ site.baseurl }}/assets/images/codecademy/line.png)
<br>
![codecademy]({{ site.baseurl }}/assets/images/codecademy/00-learn-01.png)    
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 6. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 7. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 8. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 9. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 10. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 11. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 12. 



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
### 13.



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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
<font size="3"  face="돋움">BATTLESHIP!</font> 
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
