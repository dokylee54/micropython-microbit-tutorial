# 1일차

- 교재 : 203.255.176.221 (ewha1234/ewha1234)

- 브라우저 에디터 : makecode.org – ms가 운영

***

## Microbit : microbit.org

- download = flash : 기기에 코드 입히기

  <-> arduino의 upload

**Thonny IDE :**

- microPython 있음

- 끌땐 Run-Disconnect (teraterm쓸때 끄기)

**TeraTerm:**

- 끌땐 File-Disconnect

**python:**

- Python Library : package(folder) > module(file)

- Ex) 

  ```python
  from math import * // math 안의 모든 함수를 가져오라는 의미
  
  print(sin(9))
  ```

- class > function (method or member)

-  block representation #~#

- ```python
  #
  askd
  asldkma
  #
  ```

- coding의 핵심

  sequence (=실행순서) / select (=if) / Iteration (=while)

**example code:**

[PDF] https://readthedocs.org/projects/microbit-challenges/downloads/pdf/latest/

- Microbit HW

![image-20191217152107713](/Users/dokylee/Library/Application Support/typora-user-images/image-20191217152107713.png)

- display 사용

```python
from microbit import *

while True:
  display.scroll('doky')
  display.show(Image.HEART)
  sleep(2000) # 2초 잠들기
```

```python
from microbit import *

# 0열 4행 LED를 밝기 9를 주는 코드
display.set_pixel(0,4,9) 
```

***

# 2일차

 **example code:**

[PDF] https://readthedocs.org/projects/microbit-challenges/downloads/pdf/latest/

- play music

```python
from microbit import *
import music

music.play(music.NYAN)
```

- python

   list () [] - order 존재

  set(집합) - order 없음

  self : 메모리 안의 인스턴스 안의 자기 자신의 위치를 의미

  ​		인스턴스 생성시 다 다르게 만들어짐 ->  다 다른 def, instance가 됨. 자기 스스로 펑션을 만들어낸다고 생각

  ​		self가 있다면 거의 class 생성 시 사용됨 -> 일반적인 def 에는 들어가지 않음

 

# 3일차

- python

  list : 여러 타입이 들어감 / array : 하나의 타입만 들어감

  lambda

  ```python
  '''
  함수 이름 = lambda 파라미터1, 파라미터2, ... : 함수 결과
  '''
  sum = lambda x,y : x+y
  print(sum(1,2))
  # 3
  ```

  class

  ```python
  class Parrot:
    
    # class attribute
    species = "bird"
    
    # instance attribute
    def __init__(self, name, age):
      self.name = name
      self.age = age
      
    # initiate the Parrot class
    blu = Parrot("Blu", 10)
    
    # access the attributes
    print(blu.specied, blu.name, blu.age)
  ```

  data structure

  ​	- list, tuple, dictionary, set

- ESP32

  AIoT 에 사용할 수 있는 chip

  dual core

  firmware : ROM이 들어가 있는 sw

  

  

  